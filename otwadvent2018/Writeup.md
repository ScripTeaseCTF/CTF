# otwadvent2018



### EasterEgg1

go to robots.txt

![Image 1](https://github.com/ScripTeaseCTF/CTF/blob/master/otwadvent2018/images/1.PNG)

then go to static/__s3cret.txt and scroll to bottom of the page 

![Image 1](https://github.com/ScripTeaseCTF/CTF/blob/master/otwadvent2018/images/2.PNG) 
    
![Image 1](https://github.com/ScripTeaseCTF/CTF/blob/master/otwadvent2018/images/3.PNG)

flag worth 50 points

AOTW{D0ra_th3_haxxpl0rer}


### EasterEgg2 

go to /static/js/app.js 


	...
	if(lockedcount != $scope.lockedCount) {
	  if($scope.lockedCount != -1) {
	        if(localStorage.getItem("gfx") != 2) {
		    var audio = new Audio('/static/audio/santabells.mp3');
		    audio.play();
		    $scope.showsanta = true;
			$("#santa").html(atob("PHA+QU9UV3tKaW5nbGVfQWxsX1RoZV9XYXkhISExfTwvcD4="));
		    console.log("GFX enabled");
		} else {
		    console.log("GFX disabled");
		}
		console.log("Detected new unlocked challenges");
	  }
	  $scope.lockedCount = lockedcount;
	...

base64 decode "PHA+QU9UV3tKaW5nbGVfQWxsX1RoZV9XYXkhISExfTwvcD4"

and you obtaine the flag worth 50 points 

AOTW{Jingle_All_The_Way!!!1}

# BlueWhale CTF


Title                         	| Category     | Points   | Flag
------------------------------- | ------------ | -------  | ---------------------------------------
Find me		      				|Web	     |50		|flag:{This_is_s0_simpl3}
Find		     			 	|Stego	     |50		|flag{hctf_3xF$235#\x5e3}
I was eaten by me		      	|Stego	     |50		|flag{WelcomeT3WhaleCTF}
subspecies						|Stego 		 |50 		|flag{firsttry}
Rainy day						|Stego		 |50 		|GUETCTF{Y0u_sEE_m3}
what is this 					|Stego 		 |100 		|flag{pE3kQzmaMN}
Fit whale						|Stego		 |50		|flag{youfindmeWHALE}
Angry ping 						|Stego 		 |100 		|flag{AppLeU0}
Negative film					|Stego 		 |100		|key_is_SimCTF{LSB_yinxie}
Http		 					|Web		 |50		|flag:{Y0u_ar3_s0_Car3ful}
Lowest kiss						|Stego		 |150		|flag{i love u}
IHDR 							|Stego 		 |100 		|FLAG{ihDR_ALSO_FUN}
Really moving 					|Stego		 |100		|key{catch_the_dynamic_flag_is_quite_simple}

##  Find me (web/ 50)

F12 that thing

![Image 1](https://github.com/ScripTeaseCTF/CTF/tree/master/WhaleCTF/images/findme.PNG)
flag:{This_is_s0_simpl3}


## Find 
flag{hctf_3xF$235#\x5e3}

## I was eaten by me 
strings whale1.jpg
binwalk -e whale1.jpg
cd _whale1.jpg.extracted
cat flag.txt
flag{WelcomeT3WhaleCTF}


## subspecies

flag{firsttry}

## Rainy Day 
convert Misc01.jpg out.png 
open out-2.png and voila
GUETCTF{Y0u_sEE_m3}


## what is this 
strings rabbit.jpg 
#102;&#108;&#97;&#103;&#123;&#112;&#69;&#51;&#107;&#81;&#122;&#109;&#97;&#77;&#78;&#125;
that should look familiar... its ascii so lets convert to text.
flag{pE3kQzmaMN}

## Fit Whale 
java -jar stegsolve.jar
analyze frame browser > flag is located on frame 2 
flag{youfindmeWHALE}

## Angry ping 
I used 29a.ch and changed the color component to reveale a QR code 
scan the QR code w/ wechat 
flag{AppLeU0}

## Negative film	
lets see if we can detect an lsb with zsteg, we can and it gives us the flag nice
![Image 1](https://github.com/ScripTeaseCTF/CTF/images/negativefilm.png)
key_is_SimCTF{LSB_yinxie}

## Http
![Image 1](https://github.com/ScripTeaseCTF/CTF/images/http.png)
flag:{Y0u_ar3_s0_Car3ful}

## Lowest kiss 
![Image 1](https://github.com/ScripTeaseCTF/CTF/images/lowestkiss1.png)
I want to turn the picture into png, then go to stegsolve, the QR code comes out so im shit lazy use the drawing to change the png format
![Image 1](https://github.com/ScripTeaseCTF/CTF/images/lowestkiss2.png)
scan and you get the flag
flag{i love u}

## IHDR 
According to the prompt IHDR, it is possible to modify the height, throw in the winhex modified height:
![Image 1](https://github.com/ScripTeaseCTF/CTF/images/lowestkiss1.png)
![Image 1](https://github.com/ScripTeaseCTF/CTF/images/lowestkiss2.png)
![Image 1](https://github.com/ScripTeaseCTF/CTF/images/lowestkiss3.png)
FLAG{ihDR_ALSO_FUN}

## Really moving 
Open with winhex and find the missing file header, add the file header
![Image 1](https://github.com/ScripTeaseCTF/CTF/images/reallymov1.png)
then change to the GIF image, use steg to view directly.
Because some characters may be a bit unclear, you must carefully check
![Image 1](https://github.com/ScripTeaseCTF/CTF/images/reallymov2.png)
get the string: Y2F0Y2hfdGhlX2R5bmFtaWNfZmxhZ19pc19xdWl0ZV9zaW1wbGU=
decode it and you get the flag 
key{catch_the_dynamic_flag_is_quite_simple}

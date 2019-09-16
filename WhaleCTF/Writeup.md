# otwadvent2018


Title                         	| Category     | Points   | Flag
------------------------------- | ------------ | -------  | ---------------------------------------
Find me		      				|web	     |50		|flag:{This_is_s0_simpl3}
Find		     			 	|Stego	     |50		|flag{hctf_3xF$235#\x5e3}
I was eaten by me		      	|Stego	     |50		|flag{WelcomeT3WhaleCTF}
subspecies						|Stego 		 |50 		|flag{firsttry}
Rainy day						|Stego		 |50 		|GUETCTF{Y0u_sEE_m3}
what is this 					|Stego 		 |100 		|flag{pE3kQzmaMN}
Fit whale						|Stego		 |50		|flag{youfindmeWHALE}
Angry ping 						|Stego 		 |100 		|flag{AppLeU0}
Negative film					|Stego 		 |100		|key_is_SimCTF{LSB_yinxie}

##  Find me (web/ 50)

F12 that thing

![Image 1](https://github.com/ScripTeaseCTF/CTF/images/findme.png)
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


---
layout: post
title: BadUSB With a Digispark
tags: [badusb,digispark,hid]
---

Bad USB is a term used when referring to a modified USB device that when connected to a computer, will act as a HID (Human Interface Device), like a keyboard. With the new "keyboard" installed in the system, it will simulate keystrokes in order to run pre-programmed malicius commands.

This type of attack became very popular with the release of [Rubber Ducky](https://shop.hak5.org/products/usb-rubber-ducky-deluxe), a Hak5 product that does exactly what i mentioned above. Despite being an excellent product, isn't the cheapest "toy" a hacker can afford, costing $44.99 dollars. If you don't leave in the USA like me, add some more $$$ due to taxes and maybe months for the product arrive.

I started this project because i wanted to learn more about these types of attacks, and since i couldn't affoard a Rubber Ducky, nor wanted to buy an imported product and wait 1-2 months for it to arrive, i started to search for some similar products, and so i found some work being done with Digispark and Micro Pro (next post).

With Digispark costing around $1 and Micro Pro around $3, and mostly important, i could find both of these in my country, no need for imports. 

But that's enough of talking, let's go to the fun part... but first:


{: .box-warning}
**Warning 1:** This content is for educational purposes only. Don't do wrong things with it. =)

{: .box-warning} 
**Warning 2:** I hold no responsability if any problems that may happen while you are following this post. From a brick Digispark to whatever you did wrong. =P

<br/>

## Hardware Used

All that i used for this project was:

* 1x Digispark

<img src="../img/BadUSB - Digispark.jpg" width="200"/>

* 1x Jumper wire F/F (Only needed for the fastboot mod)

<img src="../img/BadUSB - JumperFF.jpg" width="200"/>

<br/>

## Drivers and software instalation

<spacer>
#### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Step 1: Installing and Configuring Arduino IDE

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; First we gonna use Arduino IDE to write our code and then upload it to out Digispark. 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Go to the Arduino official [site](https://www.arduino.cc/en/Main/Software) and download the right setup file for your OS. While installing, there's no need to change the default options, besides the directory you want to install it.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; After installed, open Arduino IDE and go to:
```perl
 File -> Preferences -> Additional Board Manager URLs
```

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; And add the following url in the *Additional Board Manager* field:
```perl
 http://digistump.com/package_digistump_index.json
```

<img class="img-center" src="../img/BadUSB - Install 1.png" width="600"/>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Now, go to:
```perl
 Tools -> Board -> Boards Manager
```

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; In the *Boards Manager* window, select the *"Contributed"* type from the drop down menu, select **Digistump AVR Boards** package and install it.

<img class="img-center" src="../img/BadUSB - Install 2.png" width="600"/>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Now you can select

<img class="img-center" src="../img/BadUSB - Install 3.png" width="230"/>



<br/>

## Programming

<br/>

## Additional: Fast boot

<br/>

## References

- [https://www.arduino.cc](https://www.arduino.cc)
- [https://digistump.com](https://digistump.com)
- [https://digistump.com/wiki/digispark/tricks](https://digistump.com/wiki/digispark/tricks)
- [https://digistump.com/wiki/digispark/tutorials/connecting](https://digistump.com/wiki/digispark/tutorials/connecting)
- [https://digistump.com/board/index.php/topic,320.0.html](https://digistump.com/board/index.php/topic,320.0.html)
- [https://digistump.com/board/index.php?topic=175.0](https://digistump.com/board/index.php?topic=175.0)
- [https://github.com/micronucleus/micronucleus](https://github.com/micronucleus/micronucleus)
- [https://github.com/micronucleus/micronucleus/tree/v1.11/upgrade/releases](https://github.com/micronucleus/micronucleus/tree/v1.11/upgrade/releases)

IMAGE
# Introduction
One of my goals for the new year is to reduce the number of applications on my phone. However, there are many applications that I need to run on a regular basis (like my car application, vacuum cleaner, cat food, etc.), that it is difficult to fully decouple from Android OS. For this reason, I decided to install Android OS on a Raspberry Pi 5 so that it lives atop my desk and in use only when needed and allowing me to delete my applications from my personal smartphone.
# Android OS on Pi 5 Components
The following components were purchased for this project:
*  Vilros Raspberry Pi 5 Starter Kit MAX - Turbo Cooled Aluminum - (128GB Edition) - (8GB RAM) - purchased for $159.99 from: https://www.amazon.com/Vilros-Raspberry-Starter-Kit-MAX/dp/B0D232HN74/ref=sr_1_3?crid=2P7BOXQATJ26I&dib=eyJ2IjoiMSJ9.DOPSBKzDUbr_p92FPgJ0S7I_GQPuGx-2kEdYNtHX82YzEjwVX19U-FxrTyjFf1GMW7mS4XxAme2mS66pBtONwl5Oc9ZgW23N4Hj285ZBUSeGGdipj7VSn1tFj_t2PQ9Ja_jUEBykKs7ygOFvwzgFqG8eWdY0KfsUhYxljiroOwv83UOKlBB1gBEdImtrWIIx1w0KhTzjrDdKtNTDalcWRgt6sWqVlWaWTJycrEaoXlU.vulbTsX8tRrYN_3VAII8HSdWJk_5l0PEi7KnP2Bf54M&dib_tag=se&keywords=pi%2B5%2Bvilros%2Bstarter%2Bkit%2Bmax&qid=1736187449&sprefix=pi%2B5%2Bvilros%2Bstarter%2Bkit%2Bmax%2Caps%2C80&sr=8-3&th=1
*  Touch Screen Monitor with Case,ROADOM 10.1’’ Raspberry Pi Screen, IPS FHD 1024×600,Responsive and Smooth Touch,Dual Built-in Speakers,HDMI Input,Compatible with Raspberry Pi 5/4/3/Zero,Versatile Stand - purchased for $109.99 from: https://www.amazon.com/ROADOM-Raspberry-Responsive-Compatible-Versatile/dp/B0CJNKFVPY/ref=sr_1_3?crid=2SRF5ERJ1CJTO&dib=eyJ2IjoiMSJ9.tA9seA5wtEabMknYU1mHFodQQg2xb94wTEWYXwQqADLkt7dXNL441rgxp2q_h98t3_GNSlkCBu62zW5RBcMPGGi3v6Rewzl1MKM-3ocZyU3pEh5RGBjlwzwnjbhxFkj3q8dyG-2Qdh5cINVe8042PK9Z5dU-nZXJEw5pZTsOiu5VjesmZ95eJpELK1SR76e-4jxnIWWXJ7ijRYyradEvZRknHlv6TmuFZ28rVrQcmDc.OIv0AGUk3SvvRqOPKlHnNE_upohw3y2y5S2btIH41y8&dib_tag=se&keywords=roadom%2Btouch%2Bscreen%2Bmonitor%2B10.1&qid=1736187524&sprefix=roadom%2Btouch%2Bscreen%2Bmonitor%2B10.1%2Caps%2C79&sr=8-3&th=1

The total cost of the project is approximately ~$270. excluding taxes.
# Initial Assembly
This part is pretty straightforward. mount the Pi 5 on the backside of the monitor and make the appropriate connections.
# Software Installation
For the software, I settled on LineageOS because there is a lot of support online, in particular, I looked at XDAforums and found this useful guide: https://xdaforums.com/t/dev-rom-unofficial-lineageos-22-android-15-for-raspberry-pi-4-pi-5.4708480/. With that in mind, here's how I went about installing LineageOS.

1. Place the microSD card from the Pi 5 kit inside a microSD card reader and connect it to your computer.
2. Download the LineageOS 22 image for Pi 5 from: https://konstakang.com/devices/rpi5/LineageOS22/ (the one that ends in rpi5).
3. Extract the zip file and then flash the .img using Pi Imager to the microSD card.
4. Once done, put the microSD card into the Pi 5 and boot it up. You should see this:

IMAGE

5. Connect to wifi, log into your Google account, and download the relevant apps. You should be good to go!
# Tips
Make sure to extract the .zip file before flashing it. Otherwise, you'll get an error. Otherwise, this should be an easy installation!

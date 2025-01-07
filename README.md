![Image_1](https://github.com/user-attachments/assets/c3f78c5d-5bff-4457-8972-0cdcd09364ad)
# Introduction
One of my goals for the new year is to reduce the number of applications on my phone. However, there are many applications that I need to run on a regular basis (like my car application, vacuum cleaner, cat food, etc.), that it is difficult to fully decouple from Android OS. For this reason, I decided to install Android OS on a Raspberry Pi 5 so that it lives atop my desk and in use only when needed and allowing me to delete my applications from my personal smartphone.
# Android OS on Pi 5 Components
The following components were purchased for this project:
*  Vilros Raspberry Pi 5 Starter Kit MAX - Turbo Cooled Aluminum - (128GB Edition) - (8GB RAM) - purchased for $159.99 from: https://www.amazon.com/Vilros-Raspberry-Starter-Kit-MAX/dp/B0D232HN74/ref=sr_1_3?crid=2P7BOXQATJ26I&dib=eyJ2IjoiMSJ9.DOPSBKzDUbr_p92FPgJ0S7I_GQPuGx-2kEdYNtHX82YzEjwVX19U-FxrTyjFf1GMW7mS4XxAme2mS66pBtONwl5Oc9ZgW23N4Hj285ZBUSeGGdipj7VSn1tFj_t2PQ9Ja_jUEBykKs7ygOFvwzgFqG8eWdY0KfsUhYxljiroOwv83UOKlBB1gBEdImtrWIIx1w0KhTzjrDdKtNTDalcWRgt6sWqVlWaWTJycrEaoXlU.vulbTsX8tRrYN_3VAII8HSdWJk_5l0PEi7KnP2Bf54M&dib_tag=se&keywords=pi%2B5%2Bvilros%2Bstarter%2Bkit%2Bmax&qid=1736187449&sprefix=pi%2B5%2Bvilros%2Bstarter%2Bkit%2Bmax%2Caps%2C80&sr=8-3&th=1
*  Touch Screen Monitor with Case,ROADOM 10.1’’ Raspberry Pi Screen, IPS FHD 1024×600,Responsive and Smooth Touch,Dual Built-in Speakers,HDMI Input,Compatible with Raspberry Pi 5/4/3/Zero,Versatile Stand - purchased for $109.99 from: https://www.amazon.com/ROADOM-Raspberry-Responsive-Compatible-Versatile/dp/B0CJNKFVPY/ref=sr_1_3?crid=2SRF5ERJ1CJTO&dib=eyJ2IjoiMSJ9.tA9seA5wtEabMknYU1mHFodQQg2xb94wTEWYXwQqADLkt7dXNL441rgxp2q_h98t3_GNSlkCBu62zW5RBcMPGGi3v6Rewzl1MKM-3ocZyU3pEh5RGBjlwzwnjbhxFkj3q8dyG-2Qdh5cINVe8042PK9Z5dU-nZXJEw5pZTsOiu5VjesmZ95eJpELK1SR76e-4jxnIWWXJ7ijRYyradEvZRknHlv6TmuFZ28rVrQcmDc.OIv0AGUk3SvvRqOPKlHnNE_upohw3y2y5S2btIH41y8&dib_tag=se&keywords=roadom%2Btouch%2Bscreen%2Bmonitor%2B10.1&qid=1736187524&sprefix=roadom%2Btouch%2Bscreen%2Bmonitor%2B10.1%2Caps%2C79&sr=8-3&th=1

The total cost of the project is approximately ~$270. excluding taxes.
# Assembly
Place the microSD card to the side for now, and screw your Pi 5 to the back of the touchscreen.

Attach connectors for touch and HDMI as instructed by the official manual. However, power the Pi using its USB-C connector and the screen using its USB-C connector, both of which were provided with their respective devices. I make this recommendation because when I was trying to power them earlier, using a singular power supply as recommended by the official manual, it resulted in undervolting. The final connections should look like this:

![Image_2](https://github.com/user-attachments/assets/c35ca69e-7c96-4a50-8189-207ffe0ec893)
# Software Installation
For the software, I settled on LineageOS because there is a lot of support online, in particular, I looked at XDAforums and found this useful guide: https://xdaforums.com/t/dev-rom-unofficial-lineageos-22-android-15-for-raspberry-pi-4-pi-5.4708480/. With that in mind, here's how I went about installing LineageOS.

1. Place the microSD card from the Pi 5 kit inside a microSD card reader and connect it to your computer.
2. Download the LineageOS 22 image for Pi 5 from: https://konstakang.com/devices/rpi5/LineageOS22/ (the one that ends in rpi5).
3. Extract the zip file and then flash the .img using Pi Imager to the microSD card.
4. Once done, put the microSD card into the Pi 5 and boot it up. You should see this:

![Image_3](https://github.com/user-attachments/assets/203b6bd9-511c-4ee1-9166-c43a46784712)

5. Connect to wifi and follow the setup guide. If you want to restore a backup, feel free to do so. If you'd like to password protect it, you can do so too in the setup phase.You can also set how you will navigate your interface. For this, I recommend "Gesture navigation." it tends to be more natural and avoids having extra buttons at the bottom of your screen.
6. LineageOS, by default, does not come with the Play Store because it is an open source OS. This means you need to install the Play Store on your own. First, on your LineageOS install, go to: https://f-droid.org/en/
7. Click on "Download F-Droid"
8. Go to Downloads on your device and you will be faced with this creen when click on F-Droid:

![Image_4](https://github.com/user-attachments/assets/f0766150-7da0-4c73-90f2-0133fec4b7cd)

9. Go to settings to allow and then you should be prompted to install F-Droid. Open it and wait for repositories to be updated.
10. You can now install a Play Store alternative; I recommend seraching for Aurora Store:

![Image_5](https://github.com/user-attachments/assets/bc18786a-e5f2-415e-af35-53c01dde00e3)

11. You will be prompted again to give permission for F-Droid to install apps. Allow it.
12. Give permissions for Aurora Store to install apps and either sign in through Google or simply use the Aurora Store anonymously. You will now have access to all the apps you need to create your own little Android hub!

![Image_6](https://github.com/user-attachments/assets/d072f024-4014-4f2a-8c5e-f9f37111051f)

# Tips
First, make sure to extract the .zip file before flashing it. Otherwise, you'll get an error.

Second, please note that some banking apps might not work that well because they seem this installation as a security risk.

Third, a lot of apps are by default vertical. You may want to figure out a way to rotate the screen in the settings. I like running my apps as is with my interface horizontal, so I will keep it like this.

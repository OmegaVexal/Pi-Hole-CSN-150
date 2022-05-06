Hello!, I’m  David Mesa aka @OmegaVexal
I’m interested in Raspberry Pi Projects, Python/JavaScrip Programming & Scripts & Pentesting
I’m currently learning Pyhton on Udemy, Pentesting on Infosec and more Cyber Security concepts
I’m looking to collaborate on any projects to get my feet wet in the cyber sec/ IT field
You can reach me at Omegaxis15@gmail.com


# Pi-Hole-CSN-150
Steps on how to set up a Raspberry Pi into an Ad-Blocker known as a Pi-hole
First you will need a rasberry pi, any will work.
You will also need a micro-sd card, sd card reader,micro usb or usb-c cable if you have a Pi4 and onwards.
Once you have all your gear head on to <https://www.raspberrypi.com/software/> and download the Rasberry Pi imager, make sure to download the apropriate imager for your OS. Another way to install the imager is inputting <sudo apt install rpi-imager> on the terminal window.
Once your imager is downloaded open it as administrator, Insert your Microsd into the SD-CARD reader and plug it into your computer device and wait for it to load
On the imager click on "Choose OS" click on Rasberry Pi OS(other) and select Rasberry Pi OS Lite 32-bit
After you chose the OS, Click on storage device and make sure you pick the inserted SD-card
On the bottom right there will be a  "Settings Wheel" click on it and name your Rasberrypi, Enable SSH, and give it a username and password.( Make sure to remember your user name and password I suggest you take a picture of this page incase you forget.)
Once all options are selected click on "Write" and let the imager do it's thing.
Once the imager completes writing on to the card you want to download the the "wsl_supplicant.txt" file and put your SSID after the = on the corresponding field, as well as your password( this is your wifi password) after the = on the pwd field.
After you are done with that donwload the "ssh" file from the repository and put it on the root of the sd card ( This will let you SSH into the Pi)
Safely remove the sd card from the computer and insert it into the Pi, at this point you will want to connect the pi to an external power supply and insert the Ethernet cable on the pi.
Now you will want to go into your Router to find out what IP address it assigned to the Raspberry Pi, Open up your Web Browser and Type "192.168.1.1" on your address bar to connect to your router, alternatively you can type "ipconfig" on your "command promt" to make sure what the IP address of your router is, if this is your first time on this page it should be "admin" for user name and "0000" for password, if you are having difficulty with this step check your router model on google to find the best way to access the interface.
Next you will want to check your connected devices, Depending on how complex your router’s software is, you may need to do some exploring until you find a page which lists all of the devices currently connected to the network along with their IP address, this is usually called a DHCP table.The Raspberry pi should have the same name you gave it on step 16 Take note the IP address assigned to your Pi. We will need it for the next few steps
While you’re logged in, you will need to set this IP address up as a static IP address, so that your router always assigns this same address to your Raspberry Pi, Every router is different so you’ll need to do some digging if you don’t know how to set up a static IP on yours. If you can’t find the option, try googling your Router’s model and the words “static IP” and you should find some information regarding how to set a static IP.
For this step there are two ways to get the same result, using the command prompt or downloading the ssh client "PuTTY"
  

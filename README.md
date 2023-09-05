<div align="center">
<img src="https://github.com/gitclone-url/SPD-T610-Phones-Rooting-Tutorial/assets/98699436/d330bbb9-fd87-4aac-8036-83ad1cb85059">
</div>


# Notes (read first!)

- A working brain 🧠,Minimal knowledge about rooting a phone is needed. If you had never rooted a phone don't follow this guide.

- Backing up your data is necessary in case something goes wrong you will have options to recover.

- A similar tutorial [**video**](https://youtu.be/8dZZci43un8) on how to flash a single partition on spd phones from hovatek is also available you can watch it for deeply understanding my guide.
Note: Don't follow this Tutorial just watch in case if you are not understanding a single line of my guide.

- some people face spd tool errors while flashing, if you face anything like that please don't prefer youtube videos for solutions, because they don't work. if you follow them you may face worst situations rather than solving the errors, you may lost your device Imei, NVdata, networks etc..

- Follow This [**guide**](https://www.hovatek.com/forum/thread-4870.html) instead. This guide is from hovatek.com you can follow this guide to solve all types of spd tool errors.

- All this phones share many similarities so a firmware of Micromax in 2b can also be flashed in symphony z33 or in2c. If you wish to flash another firmware, Yes you can! but proceed with caution ⚠️ i don't take any responsibility in case something happens wrong. i recommend you to stick with your device firmware, it does not guaranteed that if you flash another firmware device will boot without problems. As far as on my testing both Micromax  in2b/in 2c firmware booted successfully on (symphony z33).

- Remember always use [spd upgrade tool](https://androidmtk.com/download-spd-upgrade-tool-all-versions) for flashing a full firmware in any case if your device got soft or hard bricked or any other problems occurs* all though it won't happen if you follow my guide carefully.

# Let's Begin.

#### Requirements 
• You must need a computer for this guide.

**Download the files from the below links, connect to VPN if download is not starting**

• Spd research tool from here [link](https://mega.nz/file/HodB3aBQ#yWAQkWkxaHHj0_CJFrQ4ewIYLtbUiMvxSVucwqPMePQ)

• Spd usb driver [link](https://www.mediafire.com/file/drsf5fboohhork2/SPD_Driver_R4.20.0201.zip/file)

**Download firmwares according to your device.**

• Micromax in 2b Firmware From [Here](https://micromaxstockrom.com/micromax-in-2b-e7544) 
(doesn't matter which one you download)

• Symphony z33 firmware from [Here](https://drive.google.com/file/d/13bspdVOeYJauf3F74aeWURDt_5kEU-dM/view?usp=sharing)

• Symphony z45 firmware from [Here](https://drive.google.com/file/d/17IVKd8QNeSjHqGzvoTrRxtRCo4QKaZnD/view)

• Micromax in 2c firmware from [Here](https://micromaxstockrom.com/micromax-in-2c-e6533)
(doesn't matter which one you download)

#### Backups!
Backing up your data is very important in case if something goes wrong you can recover, so it is highly recommend.
You can use Android Default data backup method for backing up your data watch this [**video**](https://youtu.be/5KVQ_-AIClc) for a detail explanation


## Flashing guide.
First of all you need a signed boot image and also a vbmeta-sign.img for rooting
You can get them from my [telegram group](https://t.me/UnisocT610Development).
![Screenshot](https://github.com/gitclone-url/SPD-T610-Phones-Rooting-Tutorial/assets/98699436/eb301029-8ecb-470e-bcfd-9a8ae3fcfa14)

Or you can use my [boot-img-puller](https://github.com/gitclone-url/Boot-img-puller) script to pull boot image from your firmware later you can use my [BIScript](https://github.com/gitclone-url/BIScript) to sign that particular image then you can flash it to your phone.if you flash without signing you will get bootloop for more info [read](https://www.hovatek.com/forum/thread-32664.html) this and [this](https://www.hovatek.com/forum/thread-32674.html).

Please note : if you use boot image and vbmeta-sign image from my telegram group then the firmware version that your phone is running on must need to matche with the provided firmware info in my pinned message **only** then you can use it.

![Screenshot](https://github.com/gitclone-url/SPD-T610-Phones-Rooting-Tutorial/assets/98699436/890829a6-1286-4fbf-bb61-52d7833e1938)


#### Extracting and installing usb driver.

First Extract Spd research tool zip on your computer then spd usb driver zip & your firmware zip file Then go in spd usb driver folder install the driver according to your windows version.

like if you have 
windows 7 you need to install it from windows 7 folder if you have windows 10 then you need to install it from windows 10 folder only if you have windows 11 running on your pc then you can also install the driver from windows 10 folder.

Installing instructions : [here](https://gsmusbdriver.com/install-spd-driver-r4-20-0201)

Detailed video : [here](https://youtu.be/AEGW24g3KxM)

After finishing driver installation process reboot your pc for once.

##### **Instructions on how to use spd research tool for flashing.**

So now that you have rebooted your pc you need go in research tool folder where you have extracted the file launch research tool.

![desktop_screenshot](https://github.com/gitclone-url/SPD-T610-Phones-Rooting-Tutorial/assets/98699436/18cce097-fae3-41d5-a6b2-eb093743d0d2)


load the firmware by clicking on the ⚙️ gear icon

![Desktop_Screenshot](https://github.com/gitclone-url/SPD-T610-Phones-Rooting-Tutorial/assets/98699436/bd37a517-fd1c-4d9d-834d-06232586b795)

you need to select a pac file, you will find it inside the firmware folder that you have extracted.

![desktop_screenshot](https://github.com/gitclone-url/SPD-T610-Phones-Rooting-Tutorial/assets/98699436/bbb82980-f52e-4ce1-8371-00c284f2a4ae)


Instructions on how to use spd research tool can be found here : `https://androidmtk.com/use-spd-research-tool` a [video](https://youtu.be/vIXylSwA_AY) is also available.

After the firmware loading is successfully done.
![desktop_screenshot](https://github.com/gitclone-url/SPD-T610-Phones-Rooting-Tutorial/assets/98699436/723778a2-e260-4c36-8714-c3676c1b9fdc)

you can now replace the images copy boot.img & vbmeta-sign.img go inside the research tool folder,you will find images folder.
![Desktop Screenshot](https://github.com/gitclone-url/SPD-T610-Phones-Rooting-Tutorial/assets/98699436/e7052925-a039-43c1-ad25-757bb799ae12)


keep going inside.. until you see those boot and others (img) files then replace the boot image and vbmeta-sign.img by pasting it.
![Desktop Screenshot](https://github.com/gitclone-url/SPD-T610-Phones-Rooting-Tutorial/assets/98699436/6d5d5a54-6c6d-43c7-9a98-030f1694454f)


**Don't close the research tool during this process!**

Then open spd research tool "download settings" from the tool you can find the option beside the packet loading option.

**On Main Page Only select [✓]** 

select [✓] boot and [✓] Vbmeta partition's as shown in the following pictures

![Desktop Screenshot](https://github.com/gitclone-url/SPD-T610-Phones-Rooting-Tutorial/assets/98699436/5f711ec4-2fea-4c58-a289-39581ac5d4ad)

![desktop screenshot](https://github.com/gitclone-url/SPD-T610-Phones-Rooting-Tutorial/assets/98699436/0471c6f7-12e7-4d15-8e62-974d4f086321)

>boot & vbmeta

- FDL1 and FDL2
will be auto selected you can't unselect them because those are needed.

---

**Important Note**

A few Micromax in 2b users have encountered issues where their device gets stuck at the boot logo or enters a boot loop after completing the flashing procedure. To resolve this problem without losing any data, it is necessary to flash only the boot logo along with vbmeta & boot. 

---

**Please note that the following step is mandatory for Micromax in2b and in2c users, while others can proceed without this step.**

select [✓] bootlogo option as shown in the picture

![Desktop_Screenshot](https://github.com/Praveenganisetti/SPD-T610-Phones-Rooting-Tutorial/assets/110226933/67cda223-03ef-4f4d-8e14-ed40877dc5d9)

Then on backup option select the three option that is marked in the image below, if not auto selected by default.
![Desktop Screenshot](https://github.com/gitclone-url/SPD-T610-Phones-Rooting-Tutorial/assets/98699436/36fa4ec8-2ecc-4798-88b1-5f629c1b0790)

Then click on 'flash operation' you can see it on right side look down and select [✓] 
 >Active write flash

![Desktop Screenshot](https://github.com/gitclone-url/SPD-T610-Phones-Rooting-Tutorial/assets/98699436/d0425958-304d-4c1f-b83f-c548c52fb7e0)


Then click **ok** Down Bellow

**Don't close the tool**

First power off the phone then connect the phone to usb cable, hold volume up and down button for few seconds.`Then click on flash button in research tool` you can leave the buttons when the tool start flashing.

**Warning ⚠️:** if the device got trun on by your mistake you will face user canceld or some other errors! So you must need to hold the volume buttons correctly.

Here is a detailed [**video**](https://youtu.be/BOxbOyqqfY0) for better understanding 

*** 

# The End
After flashing complete you can trun on the device, once you have truned it on don't trun of the device, download and install the **same magisk application** that you have used to patch the boot image.if you used my signed boot image you will find the apk link from the pinned message.After installing open the app you will be see a prompt message coming up saying Requires additional setup just click ok your phone will be rebooted automatically and done ✔️.


***That's it your device has been successfully rooted 😉 use root checker apps to check, don't forget to say thanks @PhantomXPain on Telegram***

# Disclaimer!

The guide is provided for informational purposes only. The author does not take responsibility for any damage or loss caused by using or misusing the guide. By using this guide,you acknowledge that you are solely responsible for any outcomes, including but not limited to device damage, data loss, or voided warranty.Proceed with caution and at your own risk. Ensure that you understand the potential consequences and are willing to accept them before proceeding. It is highly recommended to follow the instructions carefully and make necessary backups of your data before attempting any modifications to your device.

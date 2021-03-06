# GMS
Good morning speaker

## Good Morning Speaker Use These Applications
* WiFi - Can download .mp3 automaticly
* Bluetooth A2DP - Transmit .mp3 via bluetooth
* Light sensor - To detect light to trigger speaker

## Hardware Uses
* Raspberry Pi 3 - Which has built-in bluetooth, WiFi and GPIO
* Grove Pi+ and light sensor
* A bluetooth speaker

## Software Uses
* Raspberry Pi 3 NOOB
* BlueZ5
* Pulseaudio
* mplayer
* Grove Pi Library


## Steps:
1. Set up NOOB from
  ```
  https://www.raspberrypi.org/downloads/noobs/ 
  ```

2. Install BlueZ5, Pulseaudio and mplayer
  - Try to follow all steps in below link to get Pulseaudio run as system-wide application. 
  Don't care that pavucontrol may not catch the alsa, if you already install pavucontrol before.
  ```
  https://github.com/davidedg/NAS-mod-config/blob/master/bt-sound/bt-sound-Bluez5_PulseAudio5.txt
  ```
  or use this copy
  ```
  To be added
  ```

3. Set pulseaudio start when boot
  ```
  https://github.com/davidedg/NAS-mod-config/blob/master/bt-sound/bt-sound-Bluez5_PulseAudio5.txt
  ```
  
4. Set Bluetooth pair with your speaker

5. Try to play a .mp3 on bluetooth speaker
  ```
  mplayer *.mp3 -ao alsa
  ```
  or 
  ```
  mplayer *.mp3 -ao pulse
  ```
  
  
6. Try to download file from Google Drive from python file

7. Install GrovePi libraries
  ```
  https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/setting-software/
  ```
  
8. Set python script run in background when boot
  - Add below in etc/rc.local
  ```
  /usr/bin/python /home/pi/Desktop/blah.py &
  ```
  
  
Reference:
- http://www.linuxquestions.org/questions/linux-newbie-8/how-to-run-mplayer-in-background-with-command-line-879090/
- https://www.raspberrypi.org/forums/viewtopic.php?f=31&t=43509
 

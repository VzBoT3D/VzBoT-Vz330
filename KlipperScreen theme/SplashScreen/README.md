# KlipperScreen Boot splash screen

Guide: https://nordfpv.com/blogs/news/customising-klipperscreen-boot-up-sequence-with-a-custom-video

Put intro1 in /etc/systemd/system/splash.service and your choice of intro2 or intro3 in /etc/rc.local

(Credits to : truefranco on Discord)
![image](https://user-images.githubusercontent.com/37383368/202033571-abe721c8-5906-41ad-8e60-673ecc3e21ef.png)


# NOTE:

OMXplayer is deprecated. Please us this:

Please use cvlc with this commands, that's only choice on debian bullseye.
Need to run commands as pi user since root is not allowed to use vlc/cvlc.

/etc/systemd/system/splash.service

```
[Unit]
Description=Splash screen 
DefaultDependencies=no 
After=local-fs.target 

[Service]
User=pi
ExecStart=/bin/bash -c "DISPLAY=:0 /usr/bin/cvlc -f --quiet --no-video-title --play-and-exit --mmal-display DSI-1 /home/pi/bootvideo/intro1.mp4" &
StandardInput=tty 
StandardOutput=tty 

[Install]
WantedBy=sysinit.target
```

/etc/rc.local
```
su - pi -c "sleep 2 | DISPLAY=:0 /usr/bin/cvlc -f --quiet --no-video-title --play-and-exit --mmal-display DSI-1 /home/pi/bootvideo/intro2.mp4"
```

BOM:

- 2 X M3 Tnuts
- 2 X M3 8mm bolts
- 4 x M2 15mm bolts or self tapping screws
- 16MP mini USB Camera https://s.click.aliexpress.com/e/_DE61tTb

Instructions:
- Disconnect the camera from the PCB
- Slide the camera with the ribbon cable facing down in the front
- Connect the ribbon cable to the PCB
- Fold the ribbon cable so it fits inside the enclosure cutout
- Install the PCB and connec the USB cable

<img width="826" alt="image" src="https://github.com/VzBoT3D/VzBoT-Vz330/assets/37383368/f8c23048-324b-4397-9210-baa1169f57ba">
<img width="826" alt="image" src="https://github.com/VzBoT3D/VzBoT-Vz330/assets/37383368/a01f1a14-7f75-43b6-b79f-d2ff5cbe0f56">
<img width="826" alt="image" src="https://github.com/VzBoT3D/VzBoT-Vz330/assets/37383368/cd796e07-4838-4270-8bbe-8b2c8998c115">

Crownsnest setting:

<sub>[cam Front]
mode: ustreamer                         # ustreamer - Provides mjpg and snapshots. (All devices)  
enable_rtsp: false                      # If camera-streamer is used, this enables also usage of an rtsp server  
rtsp_port: 8554                         # Set different ports for each device!  
port: 8081                              # HTTP/MJPG Stream/Snapshot Port  
device: /dev/video0                    # See Log for available ...  
resolution:  1920x1080                  # widthxheight format  
max_fps: 5                             # If Hardware Supports this it will be forced, otherwise ignored/coerced.  
#custom_flags:                          # You can run the Stream Services with custom flags.  
#v4l2ctl:                               auto_exposure=1,exposure_absolute=1,gamma=72, # Add v4l2-ctl parameters to setup your camera, see Log what your cam is capable of.	</sub>  

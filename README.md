# Flowmotion One 

"On July 1st, 2019, we had to announce that FlowMotion was shutting down. " - 😢

So lets start to reverse engineering the flowmotion one to build a new long time supported app and keep the flowmotion one working for a long time.

## Control Codes
__Record LED:__   
Service-UUID: B11C0005-672A-8DAB-F442-A0DAB5063A98  
Values:

| Status | Hex-Value |
|--------|-----------|
| on     | 0x01		 |
| off    | 0x00		 |

__Record-/Tilt-Button Event:__  
Service-UUID: B11C0007-672A-8DAB-F442-A0DAB5063A98  
Values:

| Button | Hex-Value |
|--------|-----------|
| record | 0x100		 |
| tilt   | 0x200		 |

## Firmware
Currently there is no way to get a firmware to recover the flowmotion one. The domain and link seems to be dead [http://firmware.api.flowmotion.co/upgrades/current?applicationIdentifier=co.flowmotion.ios.flowmotion&ap                         plicationVersion=1.8.1&d?]()

## DFU/Recovery Modus
1. Follow the steps in the video: ![](flowmotion-dfu-mode.gif)
	1. Turn on
	2. Connect and remove the charging cable
	3. Press 1x the power button
	4. Connect and remove the charging cable again
2. Then the LED should light green
3. After connecting via bluetooth the LED should light blue
4. There is a recovery option in the orignal flowmotion one app for ios but no firmware is available anymore

## iOS-App
I started developing an iOS-App but then my flowmotion one died and now only lights red 😢. Bluetooth-Connections and DFU-Mode works but nothing more. If i would be able to bring it back to live e.g. flashing the firmware again, then the app development can be continued.

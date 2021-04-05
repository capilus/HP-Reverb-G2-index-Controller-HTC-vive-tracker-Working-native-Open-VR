# HP-Reverb-G2-index-Controller-HTC-vive-tracker-Working-native-Open-VR

See on Reedit: https://www.reddit.com/r/HPReverb/comments/mitnwo/hp_reverb_g2_index_controller_htc_vive_tracker/

I would like to share almost the perfect tracking without space calibration.

What you need:
 - Index / htc Controller, lighthouses
 - HTC vive tracker 1.0. 2.0 3.0 (Maybe in future tundra tracker)
 - USB extension cable or Micro usb for tracker 1.0 and 2.0 or USB C for tracker 3.0 Cable 5mt/16 ft (optional you can use dongle).

Software:
- Open VR advanced settings: https://github.com/OpenVR-Advanced-Settings/OpenVR-AdvancedSettings
- Input Emultaor with Patch: https://github.com/matzman666/OpenVR-InputEmulator/releases and https://github.com/matzman666/OpenVR-InputEmulator/issues/207 works on windows 10 last version.You can see how https://m.youtube.com/watch?v=xr9zXrS1sFg
- Steam VR beta .
  
Steps:
- install software.
- Pair your vive tracker and your controller (needs dongles)
- Open steamvr.vrsettings (typically in windows C:\Program Files (x86)\Steam\config)
- add these lines

}, 

"steamvr" : {     
   "activateMultipleDrivers" : true 

}, 
"TrackingOverrides" : {    
   "/devices/htc/vive_trackerLHR-YOURSERIAL" : "/user/head" 
}, 
"trackers" : {
   "/devices/htc/vive_trackerLHR-YOURSERIAL" : "TrackerRole_None"
}

Note: you can see your serial in input emulator in devices.

- After this when you turn on your vive tracker and steam vr you can see than you can move the screen witn the tracker. it's important to have the tracker at exact same position as it is in my picture, it won't work if it's anywhere else on your head. Don't be panic first you gonna have gray screen but after few seconds you gonna see the screen and controllers.

- i create a remix of this HMD mount: https://www.thingiverse.com/thing:4780501,  is not perfect hoping someone can do a more professional version.

- Then you have to set up steam room calibrator and use advanced settings to fix floor if you need after installation.
- Because the tracker it's around 10 cm far from your HMD you can use input emulator to fix that adding -10 to fix your controllers.
- You can use the vive tracker with the dongle but you can have some lag i recommend use a direct connection with the usb cable.
- Hope you like and add- improvement. i'm not a expert programer only a normal user who love VR and want the best imaging with the best tracking.

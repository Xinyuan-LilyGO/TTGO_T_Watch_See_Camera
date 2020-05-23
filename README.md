# View remote camera with TTGO-T-Watch

## 1. The server:

   Hardware: Raspberry Pi (with camera)
   
   Directory: raspberry_server
   
   Run: python camera_server.py
   
   Note: Some wifi cameras directly support the mjpg streaming protocol with mjpg server capability.

## 2. Client 1  

   Hardware: TTGO T-WATCH
   
   Directory: TTGO_T_Watch_See_Camera Need to adjust router account, password, Raspberry Pi IP
   
   Compilation tool arduino development board select TTGO T-Watch, set port, compile and burn to TTGO T-WATCH
   
   Operation: Turn on the computer, and after connecting to the router, press the second button to view the remote camera camera for 60 seconds
   
   Read a picture from a remote camera through an http interaction, and repeat many times
   Demo function for learning
   
   FPS is about 1, one per second, slow
   
## 3. Client 2

   Improved version above
   
   Hardware: TTGO T-WATCH
   
   Directory: TTGO_T_Watch_See_mjpg Need to adjust router account, password, Raspberry Pi IP
   
   Operation: Turn on the computer, and after connecting to the router, press the second button to view the remote camera for an unlimited time
   
   mjpg transmission protocol, request once, return jpg images infinitely, high interaction efficiency
   
   FPS is about 6, 6 frames per second, the time is mainly spent in parsing jpg and graphic display, limited to hardware level, not easy to improve
   
   Hardware effect:
   
   <img src= 'https://github.com/lixy123/TTGO_T_Watch_See_Camera/blob/master/TTGO_T_Watch_See_Camera/IMG_20200419_194214.jpg?raw=true' />
<br/>
<br/>
<img src= 'https://github.com/lixy123/TTGO_T_Watch_See_Camera/blob/master/TTGO_T_Watch_See_Camera/IMG_20200419_194835.jpg?raw=true' />
<br/>

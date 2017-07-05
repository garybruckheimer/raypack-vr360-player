# Raypack® VR 360 Player
======
           
Raypack® VR 360 Player is HTML5 based Videoplayer for 360 Video player.

Supported Browsers for Video on Demand (VOD):
- Chrome for Desktop Windows, Linux, OSX, min. >Version 48
- Chrome for iOS
- Chrome for Android
- Android OS >5 or higher required
- Safari 10.1 or higher for OSX Desktop
- Safari iOS 10 or higher for iPHone, iPad, iPod
- Firefox 54.0.1 or higher
- IE11 on Windows 7 or 8 (only Fallback MP4 360)
- IE11 on Windows 10 (will Support)
- IE Edge on Windows 10

Raypack 360 Features
--------

* Playback of Cubemap 360 Videos
* Adaptive Streaming Support incl. HLS
* Supports HLS Live & VOD 360 Streams
* Supports Byterange HLS for VOD
* Support Segment HLS for Live Streaming
* Sample-AES & AES-128 Decryption
* Alternate Audio Support
* Support for Raypack A.I. Cluster Transcoder Solutions

Installation
------------

The Player comes with 2 Javacsript tag for installation.

These tags are standard data-* Tags for configuration the player interface.

Parameter / Description

id="raypackobject"

Description: defines the name of the Raypack Object, you can change as you need this.

src="raypackjs/apploader.js?01"
Description: defines the source path of the raypack application loader. The addon "?01" is not required, but usefull when you want not that a cached version is loaded. For new version simply add a new number lik "?02" or "?03". 

data-raypack-key="free"
Description: Defines the raypack license key. Please note that the player is free as long as you do not use it for commercial projects. The free version also shows very 4 seconds the Raypack logo.

data-raypack-user="username"
Description: Defines the username for the license key. You can leave it clear for the free version.

data-raypack-url="/raypack/raypack360/postbankdemo/stich_complete_prores.json"
Description: Defines the playlist format. We support Raypack.ai json manifest. This is a manifest generate by our Raypack AI 360 Transcoder. Alternate you can use .m3u8 HLS Files as well .mp4 files.

data-raypack-player="raypack360player" 
Description: Defines the videoplayer name.

data-raypack-playersrc="raypacksource"
Description: Defines the video source of the raypack-player. Please note that you can use a standard video HTML Object here.

data-raypack-playmode="equirectangular"
Description: Defines the raypack-cdn folder path for all third-party libraries. We do not recommend that you change this if it is not required.

data-raypack-settings
Description: Raypack Player Settings Parameter: Defines the 360 parameter.

autoplay
Description: starts the player as soon as the player has loaded all components. Please note that on iPhones autostart is not allowed, you have to press 2 times the play button.

clickdrag
Description: On Desktop you can enable to click and drag inside the 360 videoplayer. Clickdrag false is that it rotates as soon as you are in the video. Clickdrag true only rotates the video when you click and hole the mouse.

initFov
Description: Defines 
      "initLon":150,
      "initLat":0,
      "maxFov":70,
      "minFov":70,
      "returnStepLon":0,
      "backToVerticalCenter": false,
      "backToHorizonCenter": false,
      "autoMobileOrientation": true
    }'


<script id="raypackobject" 
  type="text/javascript" 
  src="raypackjs/apploader.js?01"
  data-raypack-key="free" 
  data-raypack-user="onlinelib" 
  data-raypack-url="/raypack/raypack360/postbankdemo/stich_complete_prores.json"
  data-raypack-player="raypack360player" 
  data-raypack-playersrc="raypacksource"
  data-raypack-playmode="equirectangular"
  data-raypack-cdn="raypackjs"
  data-raypack-settings='{
      "autoplay":false,
      "clickdrag":true,
      "initFov":70,
      "initLon":150,
      "initLat":0,
      "maxFov":70,
      "minFov":70,
      "returnStepLon":0,
      "backToVerticalCenter": false,
      "backToHorizonCenter": false,
      "autoMobileOrientation": true
    }'

    data-raypack-streamsettings='{         
          "startPosition":0,
          "startLevel":4,
          "capLevelToPlayerSize":false,
          "debug":false,
          "initialLiveManifestSize":0,
          "maxBufferLength":30,
          "maxMaxBufferLength":10,
          "maxBufferSize":60000,
          "maxBufferHole":0.5,
          "maxSeekHole":2,
          "lowBufferWatchdogPeriod":0.5,
          "highBufferWatchdogPeriod":3,
          "nudgeOffset":0.1,
          "nudgeMaxRetry":3,
          "maxFragLookUpTolerance":0.2,
          "liveSyncDurationCount":0,
          "liveMaxLatencyDurationCount":10,
          "enableWorker":true,
          "enableSoftwareAES":false,
          "manifestLoadingTimeOut":10000,
          "manifestLoadingMaxRetry":3,
          "manifestLoadingRetryDelay":500,
          "manifestLoadingMaxRetryTimeout":14000,     
          "levelLoadingTimeOut":10000,
          "levelLoadingMaxRetry":4,
          "levelLoadingRetryDelay":500,
          "levelLoadingMaxRetryTimeout":64000,
          "fragLoadingTimeOut":20000,
          "fragLoadingMaxRetry":6,
          "fragLoadingRetryDelay":500,
          "fragLoadingMaxRetryTimeout":64000,
          "startFragPrefech":false,
          "appendErrorMaxRetry":3,
          "enableCEA708Captions":true,
          "stretchShortVideoTrack":true,
          "forceKeyFrameOnDiscontinuity":true,
          "abrEwmaFastLive":5.0,
          "abrEwmaSlowLive":9.0,
          "abrEwmaFastVoD":4.0,
          "abrEwmaSlowVoD":15.0,
          "abrEwmaDefaultEstimate":500000,
          "abrBandWidthFactor":0.8,
          "abrBandWidthUpFactor":0.7,
          "minAutoBitrate":0
    }'
  > 
 

</script>

How To
-------
1) Create an Account on raypack.ai
2) Subscribe to Live 360 Service
3) Download VR 360 Player or try your own videos with the demo player

If you need custom development, patent clearing help or other support, please contact us: https://connectlounge.de/contact

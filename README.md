vr4wp
=====

Supports Google Cardboard for Windows Phone in Unity3D

Requires the Cardboard SDK for Unity - https://developers.google.com/cardboard/unity/

For the Barrel Distortion effect, Unity Pro is required with the Image Effects package imported.

*** Setting up your scene ***

- You need to first import the Google Cardboard SDK found here - https://developers.google.com/cardboard/unity/
- Next, import the Image Effects package by going to Assets->Import Package-Image Effects
- Add the following scripts to MainCamera(or use the prefab located in vr4wp.unitypackage)
  - DeviceInputManager
  - StereoController
  - SkyboxMesh
  - MagnetSensor
- Next, add two child game objects to MainCamera and name then Camera Left and Camera Right
- Attach the CardboardEye and BarrelDistortion scripts to each stereo camera
- Select MainCamera and press the "Update Stereo Camera" button located under the StereoController component. This will position our "eye" cameras for us in relation to the main camera.
- You're done! Add some objects to the scene to orient yourself.
- 

Code credits go to:
- DeviceInputController is based off this blog post by Alexander Dezhurko - http://blog.heyworks.com/how-to-write-gyroscope-controller-with-unity3d/
- MagnetSensor.cs code is based off of Casey B's work - https://github.com/CaseyB/UnityCardboardTrigger/tree/develop

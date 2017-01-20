ARToolKitUWP-Unity
===
Unity3D package interfacing ARToolKitUWP, with C# scripts, pre-built plugin, customized inspector property, and some default streaming assets.

Author: [Long Qian](https://longqian.me/aboutme)

Date: 2017-01-20

## Scripts
- ```ARUWPNative.cs``` directly interfaces with ARToolKitUWP wrapper. It defines the entry point of native functions with parameter correctly marshaled, and various constants used for tracking configuration.
- ```ARUWPMarker.cs``` defines a marker to be tracked by ARToolKitUWP, and relates tracking result with particular GameObjects in the scene.
	* ```Editor/ARUWPMarkerEditor.cs``` customizes the Unity inspector of ARUWPMarker objects.
- ```ARUWPController.cs``` configures the behavior of ARToolKitUWP.
- ```ARUWPUtils.cs``` provides various utility functions serving the package.

## Streaming Assets
Files in this folder are shipped with the application, which means they will also be accessible during runtime. Marker configurations, pattern definition, camera calibration files are placed here.

```hololens896x504.dat``` is the camera calibration file of my HoloLens locatable camera. Details can be found in this [repository](https://github.com/qian256/HoloLensCamCalib/tree/master).

## How does it look like?
The following images are screenshots of Unity inspector of ARUWPController and ARUWPMarker.
<table>
<tr>
	<td align="center" width="50%"><img src="https://cloud.githubusercontent.com/assets/8185982/22160312/d4821bfe-df12-11e6-80cf-cfbfc7f4b5be.png" /></td>
</tr>
<tr>
	<td align="center" width="50%"><img src="https://cloud.githubusercontent.com/assets/8185982/22160313/d482b582-df12-11e6-88e3-3f1f03e0fef7.png" /></td>
</tr>
</table>

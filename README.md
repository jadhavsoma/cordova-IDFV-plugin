<h4>Deprecation notice</h4>

cordova-plugin-device now returns the Identifier For Vendor on device.uuid, so there is no point of continuing using this plugin https://www.npmjs.com/package/cordova-plugin-device

<strong>Identifier For Vendor Plugin</strong>

This plugin makes possible to get the iOS Identifier For Vendor code on phonegap apps https://developer.apple.com/library/ios/documentation/uikit/reference/UIDevice_Class/Reference/UIDevice.html#//apple_ref/occ/instp/UIDevice/identifierForVendor

On iOS 5 the error callback is called because Identifier For Vendor isn't supported on iOS 5

Installation:

cordova plugin add https://github.com/jadhavsoma/cordova-IDFV-plugin.git

Usage:
<pre>
window.IDFVPlugin.getIdentifier(function(result){
                                      alert(result);
                                    },
                                    function(error){
                                      alert(error);
                                    });
                                    </pre>

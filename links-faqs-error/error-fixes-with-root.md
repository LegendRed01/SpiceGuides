# Error Fixes \(with Root\)

## Error codes and solutions

### Error 11 NO GPS SIGNAL \[Systemized GPS App\]

* Check that **Google Play Store** is **enabled**
* Check if the **Google Play Store** is **Up-to-Date**
* Check the following settings in Fake GPS Joystick :

  * **Enable** Indirect Mocking
  * **Enable** System Mode
  * **Disable** Location Service
  * Wrap your phone in tinfoil or try it out indoors

### Error 11 NO GPS SIGNAL \[Smali Patcher\]

* Make shure your spoofing app is **not** Systemized
* Check the following settings in Fake GPS Joystick :
  * **Disable** Indirect Mocking

### Error 12 - NO GPS SIGNAL / FAILED TO DETECT LOCATION

* Disable and re-enable Google Play Services and Maps \(downgrading it in the process\)
* Disable auto updates on Google Play Services
* Set accuracy to PHONE only

##  **Smali Patcher ISSUES AND SOLUTIONS**

### !!! ERROR: Mock location class not found.

* This means that the patcher cannot find core android classes**,** this usually means your service.jar is not deodexed properly or you didn't allow for USB debugging

### !!! ERROR: BASE DIRECTORY NOT FOUND ::

* You did not accept the USB debugging permission popup on your phone. The patcher can't do anything without this permission
* The permission popup should be displayed after hitting the "ADB PATCH" button or as soon as you connect your phone to your PC
* If you can't see the permission popup: go to settings → developer options → revoke USB debugging authorizations, disconnect and reconnect your phone and try again
* Make sure you tick "always allow from this computer" otherwise, you may have to confirm the popup multiple times during a single patch

### UNSUPPORTED MAJOR.MINOR VERSION XX.X ::

* Use the Java Uninstall Tool to clean up out-of-date java versions and reinstall the latest java release

### W: COULD NOT FIND RESOURCES ::

* This is a harmless warning, you can safely ignore it.

### !!! ERROR: XYZ CLASS NOT FOUND ::

* If you are browsing for a services.jar - it's most likely not deodexed.


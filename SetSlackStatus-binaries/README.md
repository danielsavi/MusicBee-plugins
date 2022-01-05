# <img src="plugin-logo.jpg" width="48" height="48"> Set Slack Status 1.0.2

Tested under Win10/Win11 x64 - Required [MusicBee 3.x](https://www.getmusicbee.com/) and [.NET 4.5](https://www.microsoft.com/en-ca/download/details.aspx?id=30653)

* 2022-01-04 mb_setSlackStatus-1.0.2.zip
    * Channel Name setting is no longer required
    * Bug fix: slack process detection
* 2022-01-04 mb_setSlackStatus-1.0.1.zip
    * Added SetForegroundWindow - restore your Focused window
* 2022-01-03 mb_setSlackStatus-1.0.0.zip
    * First release

## Directions:

* :package: Unpack **mb_setSlackStatus-1.0.2.zip** contents into Musibee's **plugins** folder.
    * When using MSI Installer, probably: C:\Program Files (x86)\MusicBee\Plugins\
* :wrench: If doesn't work out-of-the-box. Open the plugin Settings...

![plugin-settings-win11](plugin-settings-win11.jpg)

* :point_right: Click the **Test** button. Expected result: all two Textboxes should be green.

### Example when Test has passed
![plugin-settings-win11-test-passed](plugin-settings-win11-test-passed.jpg)

### Example when Test has failed (i.e. Slack not running/detected)
![plugin-settings-win11-test-failed](plugin-settings-win11-test-failed.jpg)

* :point_right: Then click **Save** to save your changes, if any.
* :musical_note: Enjoy it :wink:

### MusicBeePortable_3_4_custom.zip

My Company's Advanced Malware Protection (AMP) is flagging the MSI installer and also the Portable version. So,
I've downloaded the [portable](https://www.getmusicbee.com/) version and manually [updated](https://www.un4seen.com/) the culprit files, listed bellow:

**bassasio.dll** : 1.4.0.2  => 1.4.1.0

**bassenc.dll**  : 2.4.14.0 => 2.4.15.0
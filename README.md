Android-Bloatware [![Status](https://travis-ci.org/jaredsburrows/Android-Bloatware.svg?branch=master)](https://travis-ci.org/jaredsburrows/Android-Bloatware)
=====
Keeping tracking of Bloatware that is safe to disable.

Original blog post: http://blog.burrowsapps.com/2014/03/what-android-apps-are-safe-to-remove.html

This list contains apps from Cyanongenmod and devices such as the Nexus 6. 

### Download the Android SDK for ADB(Android Debug Bridge):

http://developer.android.com/tools/revisions/build-tools.html

### Connect your Device and Run the Script:

**With root(disabling apps with root):**
 - `./disable-root.sh`

**Without root(attempt to disable apps without root):**
 - `./disable.sh`

### How it works and Basic Commands:

**How to list all packages:**

 - `adb shell pm list packages -f`

**How to disable apps *without* root:**

 - `adb shell pm disable <com.package.name>`

**How to disable apps *with* root:**

 - `adb root && adb shell pm disable <com.package.name>`
 or
 - `adb shell "su -c 'pm disable <com.package.name>'"`

### Success vs Unsuccessful:

**New state: disabled**

`Package com.android.dreams.basic new state: disabled`

You have successfully disabled the application.

**IllegalArgumentException**

`Error: java.lang.IllegalArgumentException: Unknown package: com.android.musicvis`

This mean your Android device does not have this application installed. 

### Packages

<table border="1"><tbody>
<tr><th>Package Name</th><th>Description</th></tr>
<tr><td></td><td></td></tr>
<tr><td>com.andrew.apollo</td><td> Music Player</td></tr>
<tr><td>com.android.apps.tag</td><td></td></tr>
<tr><td>com.android.backupconfirm</td><td> Restores Google settings</td></tr>
<tr><td>com.android.browser</td><td> Stock Browser</td></tr>
<tr><td>com.android.calendar</td><td> Stock Calendar</td></tr>
<tr><td>com.android.camera2</td><td> Stock Camera</td></tr>
<tr><td>com.android.captiveportallogin</td><td></td></tr>
<tr><td>com.android.cellbroadcastreceiver</td><td> Alert Broadcasts</td></tr>
<tr><td>com.android.development</td><td> Development App</td></tr>
<tr><td>com.android.dreams.basic</td><td> Screensaver</td></tr>
<tr><td>com.android.dreams.phototable</td><td></td></tr>
<tr><td>com.android.email</td><td> Stock Email</td></tr>
<tr><td>com.android.exchange</td><td></td></tr>
<tr><td>com.android.facelock</td><td></td></tr>
<tr><td>com.android.galaxy4</td><td></td></tr>
<tr><td>com.android.gallery3d</td><td></td></tr>
<tr><td>com.android.htmlviewer</td><td></td></tr>
<tr><td>com.android.inputdevices</td><td></td></tr>
<tr><td>com.android.inputmethod.latin</td><td></td></tr>
<tr><td>com.android.magicsmoke</td><td> Live Wallpaper</td></tr>
<tr><td>com.android.managedprovisioning</td><td> Google Workplace</td></tr>
<tr><td>com.android.mms</td><td> Stock Messaging</td></tr>
<tr><td>com.android.moto.appdirectedsms</td><td></td></tr>
<tr><td>com.android.musicfx</td><td> Audio Equalizer</td></tr>
<tr><td>com.android.musicvis</td><td> Live Wallpapers</td></tr>
<tr><td>com.android.noisefield</td><td> Live Wallpaper</td></tr>
<tr><td>com.android.pacprocessor</td><td></td></tr>
<tr><td>com.android.phasebeam</td><td> Wallpaper</td></tr>
<tr><td>com.android.printspooler</td><td></td></tr>
<tr><td>com.android.providers.downloads.ui</td><td> Downloads</td></tr>
<tr><td>com.android.providers.partnerbookmarks</td><td></td></tr>
<tr><td>com.android.providers.userdictionary</td><td> Dictionary for Keyboard</td></tr>
<tr><td>com.android.proxyhandler</td><td></td></tr>
<tr><td>com.android.quicksearchbox</td><td> Search Box</td></tr>
<tr><td>com.android.sdm.plugins.connmo</td><td></td></tr>
<tr><td>com.android.sdm.plugins.dcmo</td><td></td></tr>
<tr><td>com.android.sdm.plugins.diagmon</td><td></td></tr>
<tr><td>com.android.sdm.plugins.sprintdm</td><td></td></tr>
<tr><td>com.android.smspush</td><td> Tethering connectivity</td></tr>
<tr><td>com.android.soundrecorder</td><td> Sound Recroder</td></tr>
<tr><td>com.android.sprint.hiddenmenuapp</td><td></td></tr>
<tr><td>com.android.sprint.lifetimedata</td><td></td></tr>
<tr><td>com.android.videoeditor</td><td> Movie Studio</td></tr>
<tr><td>com.android.voicedialer</td><td> Voice Search</td></tr>
<tr><td>com.android.vpndialogs</td><td> VPN System</td></tr>
<tr><td>com.android.wallpaper.holospiral</td><td> Live Wallpaper</td></tr>
<tr><td>com.android.wallpaper.livepicker</td><td> Wallpaper Picker</td></tr>
<tr><td>com.android.wallpapercropper</td><td> Wallpaper Cropper</td></tr>
<tr><td>com.bel.android.dspmanager</td><td> Audio Equalizer</td></tr>
<tr><td>com.cyanogenmod.account</td><td> Account Manager</td></tr>
<tr><td>com.cyanogenmod.CMWallpapers</td><td> Cyanogen Wallpapers</td></tr>
<tr><td>com.cyanogenmod.eleven</td><td></td></tr>
<tr><td>com.cyanogenmod.filemanager</td><td> File Manager</td></tr>
<tr><td>com.cyanogenmod.lockclock</td><td> Lock Screen Widget</td></tr>
<tr><td>com.cyanogenmod.trebuchet</td><td> Launcher</td></tr>
<tr><td>com.cyanogenmod.wallpapers</td><td> Wallpapers</td></tr>
<tr><td>com.facebook.katana</td><td> Facebook</td></tr>
<tr><td>com.google.android.androidforwork</td><td></td></tr>
<tr><td>com.google.android.apps.books</td><td> Books</td></tr>
<tr><td>com.google.android.apps.cloudprint</td><td> Cloud Print</td></tr>
<tr><td>com.google.android.apps.currents</td><td> Currents</td></tr>
<tr><td>com.google.android.apps.docs</td><td> Drive</td></tr>
<tr><td>com.google.android.apps.docs.editors.docs</td><td> Docs</td></tr>
<tr><td>com.google.android.apps.docs.editors.sheets</td><td> Sheets</td></tr>
<tr><td>com.google.android.apps.docs.editors.slides</td><td> Slides</td></tr>
<tr><td>com.google.android.apps.enterprise.dmagent</td><td></td></tr>
<tr><td>com.google.android.apps.fitness</td><td> Fit</td></tr>
<tr><td>com.google.android.apps.gcs</td><td></td></tr>
<tr><td>com.google.android.apps.inputmethod.hindi</td><td> Hindi Keyboard</td></tr>
<tr><td>com.google.android.apps.photos</td><td></td></tr>
<tr><td>com.google.android.apps.plus</td><td> Google+</td></tr>
<tr><td>com.google.android.apps.walletnfcrel</td><td> Google Wallet</td></tr>
<tr><td>com.google.android.email</td><td> Stock Email</td></tr>
<tr><td>com.google.android.gm.exchange</td><td></td></tr>
<tr><td>com.google.android.googlequicksearchbox</td><td> Search Box</td></tr>
<tr><td>com.google.android.inputmethod.japanese</td><td> Japanese Keyboard</td></tr>
<tr><td>com.google.android.inputmethod.korean</td><td> Korean Keyboard</td></tr>
<tr><td>com.google.android.inputmethod.pinyin</td><td></td></tr>
<tr><td>com.google.android.inputmethod.piyin</td><td></td></tr>
<tr><td>com.google.android.marvin.talkback</td><td> Accessibility</td></tr>
<tr><td>com.google.android.play.games</td><td> Play Games</td></tr>
<tr><td>com.google.android.street</td><td> Street View</td></tr>
<tr><td>com.google.android.tag</td><td></td></tr>
<tr><td>com.google.android.talk</td><td> Hangouts</td></tr>
<tr><td>com.google.android.videos</td><td> Play Movies & TV</td></tr>
<tr><td>com.google.android.webview</td><td> Webview</td></tr>
<tr><td>com.google.android.youtube</td><td> Youtube</td></tr>
<tr><td>com.google.earth</td><td> Earth</td></tr>
<tr><td>com.motorola.android.buacontactadapter</td><td></td></tr>
<tr><td>com.motorola.entitlement</td><td></td></tr>
<tr><td>com.motorola.motocit</td><td></td></tr>
<tr><td>com.motorola.motosignature.app</td><td></td></tr>
<tr><td>com.motorola.service.ims</td><td></td></tr>
<tr><td>com.motorola.triggerenroll</td><td></td></tr>
<tr><td>com.motorola.triggertrainingservice</td><td></td></tr>
<tr><td>com.qualcomm.atfwd</td><td></td></tr>
<tr><td>com.qualcomm.qti.rcsbootstraputil</td><td></td></tr>
<tr><td>com.qualcomm.qti.rcsimsbootstraputil</td><td></td></tr>
<tr><td>com.qualcomm.timeservice</td><td></td></tr>
<tr><td>com.svox.pico</td><td> Text to Speech</td></tr>
<tr><td>com.tmobile.themechooser</td><td> Theme Chooser</td></tr>
<tr><td>com.tmobile.thememanager</td><td> Theme Manager</td></tr>
<tr><td>com.verizo.permissions.appdirectedsms</td><td></td></tr>
<tr><td>com.verizon.omadm</td><td></td></tr>
<tr><td>com.verizon.permissions.appdirectedsms</td><td></td></tr>
<tr><td>com.vzw.apnservice</td><td></td></tr>
<tr><td>jackpal.androidterm</td><td> Terminal Emulator</td></tr>
<tr><td>net.cactii.flash2</td><td> Flash Light</td></tr>
<tr><td>org.codeaurora.ims</td><td></td></tr>
<tr><td>org.cyanogenmod.audiofx</td><td> Audio Equalizer</td></tr>
<tr><td>org.cyanogenmod.launcher.home</td><td> Launcher</td></tr>
<tr><td>org.cyanogenmod.theme.chooser</td><td> Theme Chooser</td></tr>
<tr><td>org.cyanogenmod.themes.provider</td><td> Themes Provider</td></tr>
<tr><td>org.cyanogenmod.voiceplus</td><td> SMS through Google Voice</td></tr>
<tr><td>org.cyanogenmod.wallpapers.photophase</td><td> Live Wallpaper</td></tr>
<tr><td>org.whispersystems.whisperpush</td><td> Secure SMS integration</td></tr>
</tbody></table>

License
=========

    Copyright (C) 2015 Android-Bloatware by Jared Burrows
   
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.


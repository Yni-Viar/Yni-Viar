# Sideloading apps on Google Android after 2026-2027.
## TUTORIAL IS UNFINISHED, BECAUSE THERE ARE NO WORKING TRUSTED APPS, WHICH WORK WITH ADB.

Google recently announced, that **every Android app MUST be signed by Google**.

That means, you need to **provide personal ID, address and pay a fee(!) to Google just for creating (for example an open-source) app!**

What about homeless? What about someone, who does not want personal information leak (which may or may not lead to dangerous things, such as stalking)?

I have a tutorial to install *your own apks* on *your* device.

More are or are not coming soon.

## Tutorial 1 - anyapk.
### Requirements

- A PC (for the first time)
- Wi-Fi connection.

### Windows - first-time install
1. Firstly, [download Android platform-tools](https://developer.android.com/tools/releases/platform-tools) and [anyapk](https://github.com/sam1am/anyapk/releases/download/v0.0.5/anyapk.apk)
2. Open 🗂️ Explorer (or other file manager if installed), open your Downloads folder (by default is `%userprofile%\Downloads`, but your Downlaod folder might be in other place, see your browser settings)
3. 📦 Unzip the file into the 📂 folder of your choice.
4. 📂 Open `platform-tools-latest-windows` or something like that folder.
5. 📂 Open `platform-tools folder`.
6. On your phone/tablet:
   1. Open ⚙️ Settings app.
   2. Find `about your phone` or something like that.
   3. Search `Software version / Build number` (NOT `Android version`), or something like that.
   4. click 7 times, enabling `Developer options`, or something like that.
   5. Open the `Developer options`, toggle `USB Debugging` and `Wireless debugging` to `ON`.
7. Connect your tablet/phone to PC by USB cable.
8. Apply ADB message on your phone/tablet if exists.
9. On PC: Open your terminal app. **(Windows 11 users - click somewhere on previously opened folder and select \[>_\] `Open in Terminal`)**
10. (Not necessary) type in \[>_\] Terminal `adb devices` to ensure if works.
11. For Windows 11: Open 🗂️ new explorer tab and navigate to your apk (e.g. if you downloaded an .apk, in the default path, you need to open 📂 `%userprofile%\Downloads`), 🖱️RIGHT-click your file, and select `Copy as path`
12. type in \[>_\] Terminal `adb install ` and then, insert your anyapk path path to .apk **WITHOUT THE " !!!**. (how to do that on Windows 11, is said in p.11.) (example - `adb install %userprofile%\Downloads\anyapk.apk` (your path may be different))
13. On your Android device: Follow [this manual](https://github.com/sam1am/anyapk?tab=readme-ov-file#setup--usage) after **Setup & Usage** topic.

### Linux - first-time install

Coming soon...

### Ongoing usage

Follow [this manual](https://github.com/sam1am/anyapk?tab=readme-ov-file#installing-apk-files) after **Installing APK files** topic.

<!--
## Unfinished tutorial 2.

1. [Download and install Shizuku on your Google Android device](https://github.com/RikkaApps/Shizuku/releases)
2. Enable Developer settings buy tapping 7 times at ⚙️Settings -> About -> Software/Firmware version.
3. [Follow the instruction (p. Start via wireless debugging)](https://shizuku.rikka.app/guide/setup/)
4. Next steps are coming soon...
>
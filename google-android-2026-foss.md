# Sideloading apps on Google Android after 2026-2027.
## WARNING. THIS GUIDE MAY BE UNFINISHED. FEEL FREE TO CONTRIBUTE.

Google recently announced, that **every Android app MUST be signed by Google**.

That means, you need to **provide personal ID and address just for installing (for example an open-source) app!**

What about homeless? What about someone, who does not want personal information leak (which may or may not lead to dangerous things, such as stalking)?

Currently, I see an alternative route (I think) - it is about using ADB - this utility does (currently) allow even to install pre-Android 6 apps, which was forbidden since Android 14.

> Tutorial is currently **for Windows only**. Not working on Linux, *BSD
> and especially MacOS.
1. Firstly, [download Android platform-tools](https://developer.android.com/tools/releases/platform-tools)
2. Open 🗂️ Explorer (or other file manager if installed), open your Downloads folder (by default is `%userprofile%\Downloads` (copy this))
3. 📦 Unzip the file into the 📂 folder of your choice.
4. 📂 Open `platform-tools-latest-windows` or something like that folder.
5. 📂 Open `platform-tools folder`.
6. On your phone/tablet:
   1. Open ⚙️ Settings app.
   2. Find `about your phone` or something like that.
   3. Search `Software version / Build number` (NOT `Android version`), or something like that.
   4. click multiple times, enabling `Developer options`, or something like that.
   5. Open the `Developer options`, toggle `USB Debugging` to `ON`.
7. Connect your tablet/phone to PC by USB cable.
8. Apply ADB message on your phone/tablet if exists.
9. On PC: Open your terminal app. **(Windows 11 users - click somewhere on previously opened folder and select \[>_\] `Open in Terminal`)**
10. (Not necessary) type in \[>_\] Terminal `adb devices` to ensure if works.
11. For Windows 11: Open 🗂️ new explorer tab and navigate to your apk (e.g. if you downloaded an .apk, in the default path, you need to open 📂 `%userprofile%\Downloads`), 🖱️RIGHT-click your file, and select `Copy as path`
12. type in \[>_\] Terminal `adb install ` and then, insert your path to .apk **WITHOUT THE " !!!**. (how to do that on Windows 11, is said in p.11.) (example - `adb install C:\Users\Public\Documents\your-apk.apk` (your path will be different))
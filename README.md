# DropChat

Share files between Android phones over Wi-Fi, in a chat-style interface. No internet, no accounts, no server:
phones find each other on the local network and send straight to each other.

- Send text and any file type (multi-select), with live progress bars
- Received files are saved to **Downloads/DropChat** and open with a tap
- Chat history is kept on the device
- Keeps receiving with the screen off (shows a small "DropChat is on" notification; tap **Quit** there to stop)
- Android 10 or newer

## Get the APK

### Option A: Android Studio
1. Open this folder in Android Studio and let it sync.
2. **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
3. The file is at `app/build/outputs/apk/debug/app-debug.apk`.

### Option B: GitHub (no Android Studio needed)
1. Create a new GitHub repository and upload everything in this folder (keep the `.github` folder).
2. Open the repo's **Actions** tab, run **Build APK** (it also runs on every push).
3. When it finishes, download **DropChat-debug-apk** from the run page and unzip it.

Install `app-debug.apk` on each phone (allow "install unknown apps" when asked).

## Using it
1. Put both phones on the same Wi-Fi network, or turn on a hotspot on one and join it from the other.
2. Open DropChat on both. Each appears in the other's list within a few seconds.
3. Tap a device, then type a message or tap the paperclip to send files.

If devices don't show up (some college/office Wi-Fi blocks phones from seeing each other), use a phone hotspot,
or tap the person-plus icon and type the IP address shown on the other phone's home screen.

## Notes
- Anyone on the same network who has the app can send you files. There is no accept/decline prompt or encryption yet,
  so use it on networks you trust.
- This is the debug build (signed with the standard debug key), fine for personal use.

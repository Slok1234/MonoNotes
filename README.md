# Mono Notes — Native Android project

This is a native Kotlin Android app (not a web app / WebView). It stores notes on-device with Android SharedPreferences.

## Build APK using GitHub Actions
1. Create a GitHub repository and upload all files in this folder to it.
2. Open the repository's **Actions** tab and enable workflows if prompted.
3. Select **Build Mono Notes APK** and press **Run workflow** (or push to main).
4. When the run finishes, open it and download the **MonoNotes-debug-apk** artifact.
5. Extract the downloaded artifact; `app-debug.apk` is the installable APK. On Android, allow installing apps from your browser/files app if asked.

## Build locally
Install Android Studio with Android SDK 35 and JDK 17, then open this project and run `assembleDebug`.

Note: this environment cannot compile the APK directly because Android SDK / Gradle are not installed and external downloads are unavailable. This is a native source project plus automated build workflow, not a precompiled APK.

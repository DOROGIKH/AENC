# Drone Canceller (Android + Android Auto)

Test app: finds a steady low hum (drone) in the cabin with the phone mic and plays an
adjustable anti-phase tone through the car speakers. Controls on the phone and on the
Android Auto screen (Find drone, Tone, Auto phase, Phase / Level / Frequency).

## Build the APK

**Option A: GitHub (no installs)**
1. Create a new empty repository on github.com.
2. Upload every file and folder from this zip, including the hidden `.github` folder
   (or push with git).
3. Open the repo's **Actions** tab: "Build APK" runs automatically (about 5 minutes).
4. Open the finished run and download **DroneCanceller-apk** (a zip holding `app-debug.apk`).

**Option B: Android Studio on your PC**
1. Install Android Studio, then File > Open this folder. Let Gradle sync finish.
2. Build > Build App Bundle(s) / APK(s) > Build APK(s).
3. The APK lands in `app/build/outputs/apk/debug/app-debug.apk`.

## Install on the phone
1. Copy `app-debug.apk` to the phone and open it. Allow "install unknown apps" for your file manager.
2. Open **Drone Canceller**, tap **Start**, allow microphone and notifications.

## Show it in Android Auto (sideloaded apps are hidden by default)
1. Phone Settings > search "Android Auto" > open its settings.
2. Scroll to **Version** and tap it about 10 times > accept developer mode.
3. Top-right menu > **Developer settings** > enable **Unknown sources**.
4. Reconnect to the car. Drone Canceller appears in the app launcher.

## Use
- Start the app on the phone first (Android may not let the car screen start the mic).
- Phone near the driver's headrest. Cruise steadily, tap **Find drone + baseline**.
- Tone on, raise level to match the drone, adjust phase (or Auto phase) until Reduction is positive.
- A passenger should run it. Start with the level low.

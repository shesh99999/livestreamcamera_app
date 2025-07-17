# Live Stream Camera for Play-Cricket (Trial)

[APK Download](https://github.com/shesh99999/livestreamcamera_app/releases/download/1.0.0/livestreamcamera.1.0.0.apk) 
Youtube video for setup coming soon.

## 1. Description
The Live Stream Camera app enables UK Play-Cricket clubs to live stream their matches directly to YouTube, complete with score overlays. This unofficial app (currently in beta) aims to provide a free and accessible streaming solution for UK cricket clubs. It utilizes the phone's built-in camera and supports features like camera zoom. For optimal quality, high-end phones with 5G SIM support are recommended.

**Target Users:** UK cricket clubs ( Play-Cricket Scoring ).

Live streamed Videos : https://www.youtube.com/@KashmirRangersCC

## 2. Key Features
*   Direct RTMP streaming to YouTube Live.
*   Score overlay integration for Play-Cricket matches.
    *   **Web Source:** Automatically updates scores every 3 minutes.
    *   **Bluetooth Source:** (Avalible soon for purchase) Ball-by-ball updates via a custom dongle.
*   Selectable streaming resolutions (e.g., 1080p, 720p) with adaptive bitrate.
*   Camera zoom utilization.
*   Club ID and YouTube stream key configuration.
*   Match selection for the current day based on club ID.
*   Automatic screen dimming after 2 minutes of streaming to save power.

## 3. App Installation & Setup (User Guide - from your text)

### Install
1.  [Download](https://github.com/shesh99999/livestreamcamera_app/releases/download/1.0.0/livestreamcamera.1.0.0.apk) and install the latest APK.
2.  **Allow all permissions requested by the app.** (If missed, the app will not work, so uninstall and reinstall).

### Initial Configuration (Required Once Only)
1.  **Set Club Code:** Enter your club's Play-Cricket code https://**clubcode**.play-cricket.com. eg https://kashmirrangers.play-cricket.com has club code kashmirrangers
2.  **Set YouTube Stream URL:** Format `rtmp://x.rtmp.youtube.com/live2/<stream_key>`. Replace `<stream_key>` with your club's YouTube channel stream key.
3.  **Set Resolution:** Choose 1080p or 720p. This sets the bitrate, and adaptive bitrate is used.
4.  **Select Score Source:**
    *   **Web:** Automatically updates scores every 3 minutes.
    *   **Bluetooth:** (Coming Soon) For ball-by-ball updates using a custom dongle.

## 4. How to Stream (User Guide)

### On Game Day (UK Play-Cricket games only for now)
1.  **Schedule Stream on YouTube:** Go to `youtube.com` and schedule your live stream.
2.  **Select Match in App:** Open the app; all matches for your club scheduled for today will be listed. Select the correct match.
3.  **Adjust Resolution (Optional):** Based on your 5G SIM's upload speed (use a speed test like Google's). Recommended: 7Mbps for 1080p, 5Mbps for 720p.
4.  **Start Streaming in App:** Tap the "Start Streaming" button.
5.  **Go Live on YouTube:** On `youtube.com`, go to your scheduled stream and click "Go Live."
6.  **Share:** Share the YouTube link with friends and followers.
7.  **During Game:** The app will stream with the score overlay. Brightness will auto-dim after 2 minutes.
8.  **After Game:**
    *   Stop streaming in the app.
    *   End the stream on `youtube.com` for your scheduled stream.

## 5. Recommended Streaming Hardware (User Guide - from your text)
*   High-end phone (e.g., Samsung Galaxy S21 Ultra or newer).
*   High Tripod Stand (2.6m+), like Neewer Tripod 3m Stand.
*   Mobile tripod holder with tilt and rotate (remote control heads like Ziphon YT1200 or Soonpho ME2/ME4 are even better).
*   Ground pegs and Bungee Cords for Tripod stability in high wind
*   20,000mAh (or larger) power bank for the mobile phone.
*   **(Coming Soon)** Custom USB Dongle for ball-by-ball scoring for tablets and a remote app for the tablet.
*   **(Coming Soon)** When using dongle on tab, Need USB charger and dongle adapter to charge and connect dongle on tab in same time.

## 6. Software
*   Live Camera Streaming APK [APK Download](https://github.com/shesh99999/livestreamcamera_app/releases/download/1.0.0/livestreamcamera.1.0.0.apk) *   
*   **(Coming Soon)** For Ball by Ball overla using Custom USB Dongle, Remote app for the tablet.
*   **(Coming Soon)** Software for PCS Pro (Windows) for ball-by-ball overlay for streaming.

## 7. Permissions Required (Assumed - Please Verify/Add)
*   `android.permission.CAMERA` (To access the camera for streaming)
*   `android.permission.RECORD_AUDIO` (If streaming audio along with video)
*   `android.permission.INTERNET` (To stream to YouTube and fetch web scores)
*   `android.permission.ACCESS_NETWORK_STATE` (To check network connectivity)
*   `android.permission.WAKE_LOCK` (To keep the device awake during streaming)
*   `android.permission.WRITE_EXTERNAL_STORAGE` / `android.permission.READ_EXTERNAL_STORAGE` (If saving any configuration files or logs locally - less needed with scoped storage on newer Android)
*   `android.permission.BLUETOOTH`, `android.permission.BLUETOOTH_ADMIN`, `android.permission.BLUETOOTH_CONNECT`, `android.permission.BLUETOOTH_SCAN`, `android.permission.ACCESS_FINE_LOCATION` (For the planned Bluetooth score source feature)
*   `android.permission.FOREGROUND_SERVICE` (If streaming is handled by a foreground service to ensure reliability)
*   `android.permission.POST_NOTIFICATIONS` (If using a foreground service on Android 13+)

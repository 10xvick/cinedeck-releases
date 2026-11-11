## Civet v1.0.85

> **Civet** is a modern, lightweight, hardware-accelerated streaming client purpose-built for Android TV, Google TV, and Fire TV devices.

---

### Quick Download
* **Direct APK**: [civet.apk](https://github.com/10xvick/civettv-releases/releases/download/v1.0.85/civet.apk) (2.34 MB)
* **Metadata**: [version.json](https://github.com/10xvick/civettv-releases/releases/download/v1.0.85/version.json)
* **Contract Hash**: `54d0157f`
* **Version Code**: `85`

---

### Compatibility & Architecture

#### Supported Android OS Versions
| Property | Specification | Details |
|---|---|---|
| **Minimum OS** | **Android 7.0 (Nougat)** | API Level 24+ |
| **Target / Tested** | **Android 14 (Upside Down Cake)** | API Level 34 (fully compatible with Android 15) |
| **Supported Platforms** | **Android TV, Google TV, Fire OS 6+** | Nvidia Shield, Chromecast with Google TV, Fire TV Stick/Cube, Sony/TCL/Philips Smart TVs, Xiaomi Mi Box, Waydroid, and Android-x86 |
| **Device Coverage** | **~97%+ of all active Android TV devices worldwide** | Fully verified on both leanback and touch-enabled devices |

#### CPU Architectures (Universal APK)
Civet TV is packaged as a universal architecture-agnostic APK. All video and audio decoding is driven through Android's native hardware `MediaCodec` pipeline via AndroidX Media3 without bundled native `.so` bloat. A single APK file runs across all platforms:
* **ARM 64-bit (`arm64-v8a`)**: Nvidia Shield TV, Chromecast with Google TV (4K), modern Fire TV Cube, Sony/TCL Google TVs.
* **ARM 32-bit (`armeabi-v7a`)**: Budget Android TV boxes, Fire TV Stick Lite / 4K (older models), Amlogic/Allwinner/Rockchip chips.
* **x86_64 (`x86_64`)**: Waydroid, Android-x86 PC setups, and 64-bit desktop emulators.
* **x86 32-bit (`x86`)**: Intel Atom TV boxes and standard Android emulators.

---

### Key Features & Capabilities

* **Hardware-Accelerated Playback**: Built on AndroidX Media3 (ExoPlayer) with hardware-accelerated rendering for HLS (`.m3u8`), DASH (`.mpd`), and progressive MP4 streams.
* **Multi-Audio Renditions**: Dynamic on-demand audio language selector in the native player menu supporting alternate audio tracks, dubs, and descriptive audio.
* **Subtitles Integration**: Universal multi-language subtitle support with automatic SubDL search, external SRT/VTT parsing, and real-time timing synchronization.
* **Native Offline Downloads**: Background segmented media caching engine with progress tracking, resumable downloads, and offline playback.
* **10-Foot Spatial Navigation**: Responsive D-Pad navigation engineered for TV remotes with zero input lag, 1:1 hardware key repeat synchronization, and quick-access menu overlays (`MENU` key).
* **Multi-Server Stream Discovery**: Automatic background stream extraction across multiple servers with in-place stream recovery and quality switching.
* **Seamless In-App Self Updates**: Built-in contract checking that alerts and updates the app directly on the TV without needing manual sideloading for each version.

---

### How to Install on Android TV & Fire TV

#### Option 1: Using the "Downloader" App (Recommended for TV)
1. Install the free **Downloader** app by AFTVnews from the Google Play Store or Amazon Appstore.
2. In your TV's Settings, go to **Security & Restrictions** (or **Developer Options**) > **Install Unknown Apps**, and grant permission to **Downloader**.
3. Open **Downloader** and enter the direct APK URL:
   ```
   https://github.com/10xvick/civettv-releases/releases/download/v1.0.85/civet.apk
   ```
4. Once downloaded, select **Install**.

#### Option 2: Using ADB (From PC / Mac / Linux)
Ensure ADB debugging is enabled on your TV:
```bash
adb connect <YOUR_TV_IP_ADDRESS>:5555
adb install -r civet.apk
```

---

### Integrity & Checksums
* **Filename**: `civet.apk`
* **File Size**: `2454187 bytes` (2.34 MiB)
* **SHA-256 Checksum**:
  ```
  38835ac177a741b0835524c03d4869cf5a6f4898f7d1a94507398656faefbc92
  ```

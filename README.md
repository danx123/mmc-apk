# MMC — Macan Mobile Converter

<p align="center">
  <img src="https://img.shields.io/badge/Release-v1.1.1-FF9E0B?style=for-the-badge" alt="Release Version" />
  <img src="https://img.shields.io/badge/Platform-Android-3DDC84?style=for-the-badge&logo=android&logoColor=white" alt="Platform" />
  <img src="https://img.shields.io/badge/Architecture-Jetpack%20Compose-4285F4?style=for-the-badge" alt="Jetpack Compose" />  
</p>

A fast, offline media converter for Android. Convert **video**, **audio** and **images** on your phone, powered by FFmpeg, with batch processing, ready-made presets and full control over advanced parameters.
---
## Screenshot
<img width="720" height="1600" alt="Screenshot_2026-11-09-12-24-44-21" src="https://github.com/user-attachments/assets/c2c7bf1d-0045-4c0c-b83a-589ba78ae1dc" />

---

## Features

### Three converters in one app
- **Video** — MP4, MKV, WebM, MOV, AVI, FLV, 3GP and animated GIF
- **Audio** — MP3, AAC, M4A, FLAC, WAV, OGG and Opus (plus WMA)
- **Image** — WebP, JPEG and PNG with adjustable compression quality

### Presets
One-tap presets for the most common jobs:
- **Video:** 1080p Full HD, 720p Fast, Social & WhatsApp (under 16 MB), 4K Ultra HD, WebM (VP9), Extract Audio (MP3 320k), HEVC/H.265 size saver, lossless remux (stream copy), animated GIF
- **Audio:** MP3 (320 / 192 / 96 kbps), AAC 256k, FLAC lossless, WAV PCM, OGG Vorbis, Opus, M4A
- **Image:** WebP, high-quality JPEG, lossless PNG, 512×512 avatar, Full HD bound, 256×256 thumbnail, max storage saver

### Fine-grained control
- **Video resolution:** Original, 320p, 480p, 720p, 1080p or a custom width × height. Choosing a custom resolution switches to manual mode and un-selects the preset.
- **Custom FFmpeg parameters** with quick-insert chips (CRF, presets, FPS, bitrate, trim start/end, mute audio, stream copy and more)
- **Audio tuning:** bitrate, sample rate and channels
- **Image quality** slider

### Batch queue
- Select multiple files and convert them in one go
- Live progress, speed, FPS and ETA for each job
- Cancel a single job or the whole queue, and clean up finished jobs

### Outputs
- Browse all converted files, filter by Video / Audio / Image
- Open or share any result straight from the app
- Optional **persistent output folder** (internal storage or SD card)

### Settings
- **Hardware acceleration** (MediaCodec) for supported devices
- **Multi-threading:** Auto, or choose the number of CPU threads
- **Keep screen on** while converting
- **Language:** English, Bahasa Indonesia, or follow the system language

---

## Requirements

- Android 7.0 (API 24) or newer
- Free storage space for the converted files

---

## Installation

1. Download the MMC `.apk` file to your phone.
2. Open the file. If Android asks, allow installing apps from this source (**Install unknown apps**).
3. Tap **Install**, then open **MMC**.
4. When prompted, grant the media/storage permission so MMC can read your files and save the results.

---

## How to use

1. Pick a category: **Video**, **Audio** or **Image**.
2. Tap **Select Files** and choose one or more files.
3. Choose a **preset**, or pick an output format and tune the options yourself.
4. Tap **Start Conversion**. Progress is shown in the **Queue** tab.
5. Find your finished files in the **Outputs** tab, where you can open or share them.

### Tips
- For the smallest files, use the **HEVC / Ultra Size Saver** preset.
- To send a video on WhatsApp, use the **Social & WhatsApp** preset.
- Hardware acceleration is off by default for stability. Turn it on in **Settings** if your device supports it and you want more speed.
- Custom FFmpeg parameters override the selected preset, so use them only if you know what you need.

---

## Troubleshooting

| Problem | What to try |
|---|---|
| Conversion fails | Read the error shown on the job card in the **Queue** tab. Turn off hardware acceleration and try again. |
| Cannot find my files | Grant the media/storage permission in **Settings → Storage Access Permission**. |
| Screen turns off during a long job | Enable **Keep Screen On** in **Settings**. |
| Result is saved in an unexpected place | Check the output folder under **Settings → Persistent Storage Directory**. The default is the app's `MMC_Outputs` folder. |

---

## Credits

- Built with Kotlin and Jetpack Compose
- Conversion engine: [FFmpeg](https://ffmpeg.org/) via FFmpegKit

FFmpeg is licensed under the LGPL/GPL. This build includes GPL components.

# AR Smart Textbook

Interactive AR application that brings textbook illustrations to life with 3D models and audio.

## Download

**[Download APK from Google Drive](https://drive.google.com/file/d/1nwR97EKviTpdPMfiMbn7Vsi9opc9fA4w/view?usp=drive_link)**

**Requirements:** Android 7.0+, Camera, 100MB storage

---

##  Installation

1. Download APK from link above
2. Enable "Unknown Sources" in Settings → Security
3. Install APK
4. Grant camera permissions
5. Download & print image targets from `/Assets/ImageTargets/`

---

## How to Use

1. Launch app
2. Tap "Start AR"
3. Point camera at image target (20-40cm distance)
4. 3D model appears with audio pronunciation
5. Move phone to view from different angles

---

##  Features

- **Image Recognition**: Vuforia-powered AR tracking
- **3D Models**: Apple, Ball, Cat, Dog
- **Audio**: Native pronunciation playback
- **Interactive**: Rotate phone to explore models

---

##  Screenshots

<img src="../Images/AR_Screenshots/app_icon.png" width="200">
<img src="../Images/AR_Screenshots/ar_detection.png" width="200">

---

##  Code

### Main Scripts

**PlayAudioOnTargetFound.cs** - Plays audio when target detected
```csharp
// Listens for Vuforia tracking events
// Plays assigned audio clip on detection
// Stops audio when tracking lost
```

**RotateObject.cs** - Rotates 3D model smoothly
```csharp
// Rotates model at 30°/sec on Y-axis
// Frame-rate independent using Time.deltaTime
```

---

##  Testing

**Test the following:**
- [ ] Camera starts immediately
- [ ] All 4 targets detected within 3 seconds
- [ ] Audio plays clearly
- [ ] Models rotate smoothly
- [ ] Tracking stable in good lighting

---

##  Tech Stack

- Unity 2022.3 LTS
- Vuforia Engine AR SDK
- C# Scripting
- Android SDK

---

##  Troubleshooting

**Image not detected?**
- Check lighting (avoid glare)
- Hold phone 20-40cm from target
- Print target at 300 DPI minimum

**Audio not playing?**
- Check device volume
- Verify media volume (not ringer)

**App crashes?**
- Ensure Android 7.0+
- Free up RAM (close apps)
- Reinstall APK

---
**Institution:** MITS Gwalior

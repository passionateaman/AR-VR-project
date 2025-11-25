# VR Shooting Game

Immersive VR shooting game with physics-based mechanics for Meta Quest 2.

##  Download

**[Download APK from Google Drive](https://drive.google.com/file/d/1gIz_R0ckHxdzdcj4ipm71Xo_tCQdikTE/view?usp=sharing)**

**Requirements:** Meta Quest 2/Pro, SideQuest or ADB, 150MB storage

---

##  Installation

### Using SideQuest (Easy)
1. Enable Developer Mode on Quest 2 ([Guide](https://developer.oculus.com/))
2. Install [SideQuest](https://sidequestvr.com/) on PC
3. Connect Quest via USB
4. Allow USB debugging on headset
5. Drag APK into SideQuest
6. Find in Library → Unknown Sources

### Using ADB
```bash
adb devices
adb install VR_ShootingGame.apk
```

---

## How to Play

1. Put on Quest 2 headset
2. Launch from Unknown Sources
3. **Grab gun**: Reach with right hand, press Grip button
4. **Aim**: Point at red cubes
5. **Shoot**: Pull Trigger button
6. **Score**: Watch floating UI for score updates

---

##  Features

- **Full VR Tracking**: 6DOF head and hand tracking
- **Physics Shooting**: Realistic bullet trajectories
- **Target System**: Destructible cubes
- **Score Tracking**: Real-time world-space UI
- **Performance**: 72+ FPS on Quest 2

---

## 📸 Screenshots

<img src="../Images/VR_Screenshots/gameplay_1.png" width="300">
<img src="../Images/VR_Screenshots/shooting_action.png" width="300">

---

##  Code

### Main Scripts

**GunShoot.cs** - Shooting mechanics
```csharp
// Instantiates bullet on trigger press
// Applies forward force using Rigidbody
// Auto-destroys bullets after 3 seconds
```

**Bullet.cs** - Collision detection
```csharp
// Detects collision with targets
// Destroys target and updates score
// Self-destructs on impact
```

**ScoreManager.cs** - Score system
```csharp
// Manages current score
// Updates TextMeshPro UI
// Public AddPoint() method for bullets
```

---

##  Testing

**Test the following:**
- [ ] Headset tracking smooth (no drift)
- [ ] Controllers tracked accurately
- [ ] Gun grabs reliably
- [ ] Bullets fire on trigger
- [ ] Targets destroyed on hit
- [ ] Score updates correctly
- [ ] 72+ FPS maintained

---

##  Tech Stack

- Unity 2022.3 LTS
- XR Interaction Toolkit
- OpenXR Plugin
- C# Scripting

---

##  Troubleshooting

**App won't install?**
- Enable Developer Mode
- Check USB debugging allowed
- Try different cable/port

**Controllers not working?**
- Check battery levels
- Re-pair in Quest settings

**Gun won't grab?**
- Press Grip (side button, not trigger)
- Move hand closer to gun

**Poor performance?**
- Restart headset
- Close background apps
- Check for overheating

---

##  Performance

- **Frame Rate**: 72-90 FPS
- **Memory**: ~1.5GB RAM
- **Battery**: ~2 hours gameplay

---

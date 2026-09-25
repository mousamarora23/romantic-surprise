# Romantic Interactive Surprise Website ❤️

An emotional, cinematic, and interactive romantic surprise single-page web experience built with pure HTML5, CSS3, and vanilla JavaScript.

---

## 📁 Project Structure

```
romantic-surprise/
├── index.html            # Complete website (HTML + CSS + JavaScript)
├── README.md             # Guide & documentation
├── server.js             # Local development server with video/audio range streaming
└── assets/               # Media folder containing real photos, videos, and music
    ├── music.mp3
    ├── WhatsApp Image 2026-09-25 at 11.25.54 AM.jpeg
    ├── WhatsApp Image 2026-09-25 at 11.25.54 AM (1).jpeg
    ├── WhatsApp Image 2026-09-25 at 11.25.54 AM (2).jpeg
    ├── WhatsApp Image 2026-09-25 at 11.25.54 AM (3).jpeg
    ├── WhatsApp Video 2026-09-25 at 11.44.45 AM.mp4
    ├── WhatsApp Video 2026-09-25 at 11.45.38 AM.mp4
    ├── WhatsApp Video 2026-09-25 at 11.45.55 AM.mp4
    └── WhatsApp Video 2026-09-25 at 11.45.55 AM (1).mp4
```

---

## 🛠️ Configuration Settings

All customizable options are centralized in the `CONFIG` object inside `index.html`:

```javascript
const CONFIG = {
  // 1. Password to unlock the surprise
  password: "BABY",

  // 2. Background music file path & volume (0.0 to 1.0)
  music: "assets/music.mp3",
  musicVolume: 0.45,

  // 3. 4 Photos in sequence
  photos: [
    "assets/WhatsApp Image 2026-09-25 at 11.25.54 AM.jpeg",
    "assets/WhatsApp Image 2026-09-25 at 11.25.54 AM (1).jpeg",
    "assets/WhatsApp Image 2026-09-25 at 11.25.54 AM (2).jpeg",
    "assets/WhatsApp Image 2026-09-25 at 11.25.54 AM (3).jpeg"
  ],

  // 4. 4 Videos in sequence
  videos: [
    "assets/WhatsApp Video 2026-09-25 at 11.44.45 AM.mp4",
    "assets/WhatsApp Video 2026-09-25 at 11.45.38 AM.mp4",
    "assets/WhatsApp Video 2026-09-25 at 11.45.55 AM.mp4",
    "assets/WhatsApp Video 2026-09-25 at 11.45.55 AM (1).mp4"
  ],

  // Media durations (in milliseconds)
  photoDuration: 4000,   // Display each photo for 4 seconds
  videoDuration: 7500,   // Play each video for 7.5 seconds
  orbitLoops: 1,         // Number of complete loops before the grand finale

  // Step 1: Password screen texts
  introTitle: "A Little Secret ❤️",
  introSub: "Enter the password to unlock something special...",
  errorWrongPwd: "Hmm... that's not it ❤️",

  // Step 3: Typewriter opening text
  typewriterText: 
`I don't really know when it happened.

Maybe it was one conversation.
Maybe it was one smile.
Maybe it was simply the way you became
someone I started looking forward to.

Some people enter your life quietly...
and somehow become a favourite part of it.`,

  // Step 4: Romantic message
  romanticTitle: "Maybe you're my favourite person. ❤️",
  romanticBody: 
`I don't know where this little story goes...
But I know one thing...
I'm really glad I met you.`,
  romanticButton: "Keep this secret 🤫",

  // Step 7: Periodic emotional messages during media orbit
  orbitMessages: [
    "I MISS YOU ❤️",
    "Wish you were here...",
    "Some people just become special without even trying.",
    "You mean more to me than you probably realize."
  ],

  // Step 10: Final closing messages
  finalTitle: "I LOVE YOU ❤️",
  finalSubtitle: 
`No matter how many times I say it,
it still doesn't feel like enough.`,
  finalClosing: "❤️ Forever yours."
};
```

---

## ⚡ Features & Controls
- **Password Unlock:** Password is set to `BABY` (case-insensitive).
- **Audio Control:** Top-right corner floating button to mute/unmute at any time.
- **Typewriter Fast-Forward:** Tap anywhere on the typewriter card to reveal the complete text immediately.
- **3D Orbit Sequence:** Automatically alternates between photos and videos.
- **"Next ❤️" Button:** Inside the 3D orbit section, tapping "Next ❤️" immediately transitions to the grand finale "I LOVE YOU ❤️" scene.
- **Replay:** Tap "Replay Experience ↺" in the finale to re-experience the surprise.

---

## 🚀 Running Locally
```bash
# In romantic-surprise directory:
node server.js
```
Open:
- On your computer: `http://localhost:3000`
- On your phone (same Wi-Fi): `http://<your-local-ip>:3000`

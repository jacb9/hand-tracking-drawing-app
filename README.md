# 🖐️ Hand-Tracking Drawing App

This is a browser-based HTML5 app that lets you draw on a canvas using **your index finger** and a webcam. Hand tracking is powered by **MediaPipe Hands**.

---

## 🚀 Features

- 📸 Real-time camera input
- ✍️ Draw with your index finger on the screen
- 🎨 Pinch gesture (thumb + index finger) toggles brush color (lime ↔ magenta)
- 🧼 Open palm gesture clears the canvas
- 👁️ Visual feedback for hand landmarks
- 🧰 On-screen UI controls for color and brush size

---

## ✅ How to Use

1. **Open the app in a secure browser (HTTPS required)**
2. **Grant camera access** when prompted
3. Hold your hand up so your **index finger** is visible
4. Move your index finger to start drawing
5. **Pinch gesture (index + thumb tip)** to change brush color
6. **Open palm gesture (all fingers extended)** to clear the canvas
7. Use the on-screen UI to pick a color and adjust brush size manually

---

## 🧠 How It Works

- Uses `navigator.mediaDevices.getUserMedia` for camera access
- Detects hand landmarks using **MediaPipe Hands**
- Maps the index fingertip (landmark 8) to canvas coordinates
- Tracks gestures:
  - **Pinch** = distance between index (8) and thumb (4) below threshold
  - **Open palm** = finger tips (8, 12, 16, 20) above wrist (0)
- Syncs on-screen color/size controls with gesture events

---

## ⚙️ UI Controls

- 🎨 **Color Picker**: change brush color manually
- 📏 **Brush Size Slider**: adjust stroke thickness from 1–20px

---

## ⚠️ Troubleshooting

- Make sure you're visiting over `https://` (not `file://` or `http://`)
- Check camera permissions in your browser settings
- Use on desktop for best performance (mobile is experimental)

---

## 📄 License
MIT License

---

Made with ❤️ using HTML5 + MediaPipe

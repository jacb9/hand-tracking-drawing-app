# 🖐️ Hand-Tracking Drawing App

This is a browser-based HTML5 app that lets you draw on a canvas using **your index finger** and a webcam. Hand tracking is powered by **MediaPipe Hands**.

---

## 🚀 Features

- 📸 Real-time camera input
- ✍️ Draw with your index finger on the screen
- 🖐️ Multi-hand support — draw with both hands
- 🧠 Gesture control:
  - ✴️ Pinch (thumb + index) toggles color per hand
  - 🖐️ Open palm gesture clears the canvas
- 🎨 On-screen UI:
  - Brush color selector
  - Brush size slider
  - Save drawing button (PNG download)
- 👁️ Visual feedback showing hand landmarks

---

## ✅ How to Use

1. **Open the app in a secure browser (HTTPS required)**
2. **Grant camera access** when prompted
3. Use your index finger to draw on the canvas
4. Use **two hands** to draw in parallel — each hand has its own brush color
5. **Pinch gesture** (thumb + index finger) switches your hand's brush color
6. **Open palm gesture** clears the entire canvas
7. Use the UI to manually change color or brush size, or save your work

---

## 🧠 How It Works

- Uses `getUserMedia` to capture webcam
- Detects up to **2 hands** using **MediaPipe Hands**
- Tracks the index fingertip (`landmark 8`) and draws on a canvas
- Recognizes:
  - **Pinch gesture** → toggles color per hand
  - **Open palm** → clears canvas
- Stores stroke positions and colors per hand

---

## 💾 Save Your Drawing
- Click **"Save Drawing"** to download the canvas as a PNG

---

## ⚠️ Troubleshooting
- Make sure you're visiting via `https://`, not `file://` or `http://`
- Check that the browser has access to your webcam
- Refresh the page if the camera feed stalls

---

## 📄 License
MIT License

---

Made with ❤️ using HTML5 + MediaPipe

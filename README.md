# Emotion Detector AI - README

A fast, privacy-first, browser-based emotion detection tool powered by **face-api.js** and **JavaScript**.

## 🚀 Features

* **Real-time Emotion Detection** via webcam
* **Fast & lightweight** using `TinyFaceDetector`
* Fully **client-side**: No server, no data sent anywhere
* Beautiful UI with **TailwindCSS** & emoji-based feedback

## 🧠 How It Works

1. Loads pre-trained models from `@vladmandic/face-api`
2. Accesses the user's webcam with permission
3. Detects facial landmarks & expressions using TinyNet
4. Analyzes the dominant emotion and displays the result

## 🖼️ UI Design

* **Video feed** mirrored for natural webcam feel
* **Canvas overlay** for detection (not drawn by default)
* **Emoji display** and label for emotion
* **Loading spinner** for feedback

## 🎭 Supported Emotions

* Happy 😄
* Sad 😢
* Angry 😠
* Surprised 😲
* Disgusted 🤢
* Fearful 😨
* Neutral 😐

## 📁 File Structure

```
index.html       # Main HTML file
face-api.min.js  # Loaded via CDN
```

## 🌐 Requirements

* Modern web browser with camera access (Chrome, Edge, Firefox)
* Internet connection to load face-api models (via CDN)

## 📦 CDN Models Used

```
https://cdn.jsdelivr.net/npm/@vladmandic/face-api/model
```

## 🛡️ Privacy

* All detection is done **locally** in-browser.
* No data is sent to any server.
* Works fully offline after models are loaded.

## ⚠️ Troubleshooting

* **Camera blocked**: Allow camera access in browser.
* **Autoplay error**: Click on the video feed to enable it.
* **Face not detected**: Ensure good lighting and keep face within frame.

## 🛠️ To Improve / Extend

* Add **screenshot** button to capture frame
* Use `drawFaceExpressions` to visualize detections
* Allow **model switch** (MobileNet / SsdMobilenetv1)
* Add **audio feedback** for accessibility

## 📚 Credits

* [face-api.js by @vladmandic](https://github.com/vladmandic/face-api)

---

Built with ❤️ to showcase the power of browser-based AI without compromising privacy.

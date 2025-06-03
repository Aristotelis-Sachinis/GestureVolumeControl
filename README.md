# 🖐️ Gesture Volume Control

A Python project that allows you to control your system volume using hand gestures captured via your webcam. It combines computer vision with audio control by leveraging **OpenCV**, **MediaPipe**, and **PyCaw**.

---

## 📁 Project Files

- `GestureVolumeControl.py` — The main script that captures your hand movements and adjusts the system volume.
- `HandTrackingModule.py` — A helper module that uses MediaPipe to detect and track hand landmarks.

---

## 🎯 Features

- Real-time hand detection using your webcam.
- Tracks finger landmarks (thumb and pinky).
- Calculates distance between two fingertips to adjust system volume.
- Displays live FPS and volume percentage overlay on the webcam feed.
- Visual feedback with circles, lines, and a volume bar.

---

## 📦 Requirements

Install the required Python libraries using:

```bash
pip install opencv-python mediapipe pycaw comtypes numpy
```

✅ Important: mediapipe works best with Python 3.7–3.10. If you're using Python 3.11 or later, consider switching to an earlier version.

---

## 🚀 How to Run
* Clone or download the repository.

* Ensure both GestureVolumeControl.py and HandTrackingModule.py are in the same directory.

* Run the main script:

```bash
python GestureVolumeControl.py
```

---

## ⚙️ How It Works
* The script opens your webcam feed.

* Uses MediaPipe to detect your hand and locate key landmarks.

* Calculates the distance between the thumb tip (ID 4) and pinky tip (ID 20).

* This distance is mapped to the system's volume range using PyCaw.

* A volume bar and percentage are drawn on screen for real-time feedback.

---


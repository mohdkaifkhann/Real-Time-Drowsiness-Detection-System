# 🚗 Real-Time Driver Drowsiness Detection System

A real-time computer vision based Driver Drowsiness Detection System developed using **Python, OpenCV, Dlib, and Facial Landmark Detection**. The system continuously monitors the driver's eyes through a webcam and triggers an alarm whenever prolonged eye closure is detected, helping reduce road accidents caused by driver fatigue.

---

## 📌 Features

- Real-time face detection
- Eye detection using Dlib facial landmarks
- Eye Aspect Ratio (EAR) based drowsiness detection
- Instant alarm when drowsiness is detected
- Works with spectacles
- Lightweight and real-time performance

---

## 🛠 Tech Stack

- Python
- OpenCV
- Dlib
- NumPy
- Imutils
- Scikit-learn

---

## 📷 Project Screenshots

### Eye Detection

<p align="center">
<img src="Images/1.png" width="700">
</p>

The system successfully detects both eyes in real time using facial landmark detection.

---

### Drowsiness Alert

<p align="center">
<img src="Images/2.png" width="700">
</p>

When the driver's eyes remain closed for multiple consecutive frames, the system classifies the driver as drowsy and immediately triggers an alarm.

---

## 📊 Testing & Results

<p align="center">
<img src="Images/3.png" width="900">
</p>

### Test Summary

| Test Case | Result |
|------------|--------|
| Normal Eyes Open | ✅ Passed |
| Normal Blink | ✅ Passed |
| Eyes Closed | ✅ Alert Triggered |
| Yawning | ✅ Detected |
| Low Light | ✅ Passed (Minor Delay) |
| Head Tilt | ⚠ Reduced Accuracy |

Overall Detection Accuracy: **Approximately 92%** under different testing conditions.

---

## ⚙ Installation

Clone the repository

```bash
git clone https://github.com/MohdKaifKhann/Real-Time-Drowsiness-Detection-System.git
```

Go to project directory

```bash
cd Real-Time-Drowsiness-Detection-System
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the project

```bash
python Real-Time-Drowsiness-Detection-System.py --shape-predictor shape_predictor_68_face_landmarks.dat --alarm Alert.wav
```

---

## 🧠 Working Algorithm

1. Capture live video from webcam.
2. Detect driver's face.
3. Extract facial landmarks using Dlib.
4. Locate both eyes.
5. Calculate Eye Aspect Ratio (EAR).
6. Monitor eye closure for consecutive frames.
7. Trigger alarm if drowsiness is detected.

---

## 🚀 Future Improvements

- Mobile application support
- Deep Learning based eye state classification
- Head pose estimation
- Yawning detection using Mouth Aspect Ratio (MAR)
- Better performance under low-light conditions

---

## 📚 References

- OpenCV Documentation
- Dlib Documentation
- PyImageSearch Facial Landmark Tutorials
- IEEE Research Papers on Driver Drowsiness Detection

---

## 👨‍💻 Author

**Mohd Kaif Khan**

- GitHub: https://github.com/MohdKaifKhann
- LinkedIn: https://www.linkedin.com/in/mohd-kaif-khan-96a351271

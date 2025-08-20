# Basic Hand Tracking (OpenCV + MediaPipe)

A simple **hand tracking** project built with **Python**, **OpenCV**, and **Google MediaPipe** as part of a self-improvement exercise (2022).  
This program detects hands in real-time using a webcam and draws landmarks with FPS display.

---

## Features

- **Real-time hand detection**
- **Tracks up to 2 hands simultaneously**
- **Draws hand landmarks and connections**
- **Displays live FPS on screen**
- **Press 'q' to quit**

---

## Requirements

- **Python 3.6+**
- **OpenCV**
- **MediaPipe 0.8.3.1**

Install dependencies using pip:
```bash
pip install opencv-python mediapipe
```

---

## How to Run

1. Clone or download the project:
```bash
git clone https://github.com/Brkberber/basic-hand-tracking.git
cd basic-hand-tracking
```

2. Make sure the following file is present:
   - `main.py` (the script)

3. Run the program:
```bash
python main.py
```

---

## File Structure

```
basic-hand-tracking/
│
├── main.py       # Main hand tracking code
└── README.md     # Project documentation
```

---

## How It Works

- Captures video frames using `cv2.VideoCapture(0)`.
- Converts frames to RGB for MediaPipe processing.
- Detects hand landmarks with `mp.solutions.hands`.
- Draws landmarks and connections using `mpDraw.draw_landmarks()`.
- Shows FPS counter in top-left corner.

---

## Future Improvements

- Add gesture recognition (e.g., counting fingers).
- Integrate with other OpenCV projects.
- Improve UI for better visualization.

---

## License

This project is open-source and free to use for learning purposes.

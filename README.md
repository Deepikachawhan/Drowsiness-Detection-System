# Drowsiness Detector

A real-time drowsiness and blink detection system using computer vision and facial landmark analysis. The system uses a webcam to monitor the user's eyes and triggers an alarm if drowsiness is detected.

## Features
- Real-time eye blink and drowsiness detection
- Uses facial landmarks for accurate eye tracking
- Histogram equalization for robust detection under varying lighting
- Audible alarm when drowsiness is detected

## Requirements
- Python 3.x
- OpenCV
- dlib
- numpy
- scipy
- playsound
- Pre-trained dlib facial landmark model (`shape_predictor_70_face_landmarks.dat`)

## Installation
1. Clone this repository or download the files.
2. Install the required Python packages:
   ```bash
   pip install opencv-python dlib numpy scipy playsound
   ```
3. Download the dlib facial landmark model and place it in a `models` directory:
   - [Download link](http://dlib.net/files/shape_predictor_70_face_landmarks.dat.bz2)
   - Extract the `.dat` file and put it in `models/`.

## Usage
1. Ensure your webcam is connected.
2. Run the script:
   ```bash
   python blinkDetect.py
   ```
3. If drowsiness is detected, an audible alarm (`alarm.wav`) will sound.

## Files
- `blinkDetect.py` - Main script for detection
- `alarm.wav` - Alarm sound played on drowsiness


## Credits
- Uses dlib's facial landmark detection
- OpenCV for image processing

## License
This project is for educational purposes.

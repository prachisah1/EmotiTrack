# EmotiTrack: Emotion Detection System

## Overview
**EmotiTrack** is a real-time emotion detection system that uses **OpenCV** and deep learning to analyze facial expressions and detect emotions. This project is designed to interpret human emotions such as happiness, sadness, anger, surprise, and more through facial expression recognition. It can be applied in various domains like mental health analysis, customer feedback, and human-computer interaction.

---

## Features
- **Real-Time Emotion Detection:** Captures and analyzes emotions from live camera feed or pre-recorded videos.
- **Emotion Categories:** Detects emotions such as Happy, Sad, Angry, Neutral, and Surprise.
- **Pretrained Models:** Utilizes deep learning models trained on datasets like FER2013.
- **User-Friendly Interface:** Easy-to-use interface for running the system and viewing results.

---

## Installation

### Prerequisites
Ensure you have the following installed:
1. Python (>=3.7)
2. pip (Python package manager)

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/EmotiTrack.git
   cd EmotiTrack
   ```
2. Create a virtual environment (optional but recommended):
   ```bash
   python -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## How It Works
1. **Face Detection**:
   - Uses OpenCV's Haar cascades or Dlib to detect faces in an image or video feed.
   
2. **Emotion Classification**:
   - A pretrained deep learning model (e.g., CNN) analyzes facial features and classifies the detected emotion.

3. **Visualization**:
   - Detected emotions are displayed in real time on the video feed with bounding boxes around the face.

---

## Usage

### Running the Emotion Detector
1. Open your terminal and navigate to the project directory.
2. Run the following command:
   ```bash
   python emotitrack.py
   ```
3. Follow the on-screen instructions to use your webcam or load a video file.

### Example
To run the detector on a sample video file:
```bash
python emotitrack.py --video path/to/video.mp4
```

To use the webcam for real-time emotion detection:
```bash
python emotitrack.py --live
```

---

## Technologies Used
- **Programming Language:** Python
- **Computer Vision Library:** OpenCV
- **Deep Learning Framework:** TensorFlow/Keras
- **Pretrained Models:** FER2013-based CNN
- **Visualization:** Matplotlib for plotting results

---

## Dataset
The model is trained on the [FER2013](https://www.kaggle.com/datasets/msambare/fer2013) dataset, which contains 35,887 grayscale images of facial expressions categorized into 7 emotions:
1. Happy
2. Sad
3. Angry
4. Neutral
5. Fear
6. Disgust
7. Surprise

---

## Results
- **Accuracy:** Achieved 78% accuracy on the validation dataset.
- **Performance:** Real-time emotion detection at ~30 FPS (frames per second) on a standard webcam.

---

## Future Improvements
1. Add support for multi-face detection and emotion recognition.
2. Expand emotion categories to include more complex emotions.
3. Integrate with APIs for sentiment analysis and mental health insights.
4. Develop a mobile-friendly version.

---


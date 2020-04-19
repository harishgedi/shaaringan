# Introduction

In this pet project, I use dlib to predict facial landmarks, then extract eyes from face and finally make transform the eyes into special eyes in Naruto anime.

# Installation

```bash
git clone https://github.com/baoanh1310/sharingan.git
cd sharingan
pip install -r requirements.txt
```

# How to run?

## 1. If you want to predict facial landmarks from input image
```bash
python facial_landmarks.py --shape-predictor shape_predictor_68_face_landmarks.dat --image images/sample.jpg
```

## 2. If you want to predict facial landmark in real-time video stream
```bash
python facial_landmarks_stream.py --shape-predictor shape_predictor_68_face_landmarks.dat
```

## 3. If you want to extract face parts from input image
```bash
python extract_parts.py --shape-predictor shape_predictor_68_face_landmarks.dat --image images/elon.jpg
```

## 4. If you want to count your eye blink in real-time video stream
```bash
python eye_blink_detect.py --shape-predictor shape_predictor_68_face_landmarks.dat
```

# References

## 1. Dlib

I use this library to detect face, facial landmarks and extract face parts.

## 2. Papers

If you really want to know the details in the libraries or functions in my code, I recommend you read the following papers:

- One millisecond face alignment with an ensemble of regression trees: https://bit.ly/2RPUwtD

- Real-Time Eye Blink Detection Using Facial Landmarks: https://bit.ly/3bmdqzV

EMO Mirror — Real-Time Emotion Recognition & Music Recommendation System

A smart mirror built on Raspberry Pi that recognizes a user's facial emotion in real time and recommends music to match their mood, with Amazon Alexa integration for hands-free voice interaction. Built as a team project at Velammal Engineering College (2024); findings co-authored and published in the International Journal of Science and Management Studies (IJSMS), 2024.

What it does
Captures live video via a camera connected to a Raspberry Pi.
Classifies the user's facial expression into one of 7 emotions: happy, sad, angry, fear, disgust, surprise, neutral.
Recommends and plays music matched to the detected mood.
Supports voice interaction through Amazon Alexa integration.
Displays the detected mood and recommendations on a connected screen.
My role — ML/Technical Lead

I designed and trained the emotion-recognition model:

Used MobileNet, a lightweight CNN architecture, with transfer learning on the FER-2013 dataset (48×48 grayscale facial images) to classify facial expressions into 7 emotion categories.
Chose MobileNet specifically for its low computational footprint, making real-time inference practical on Raspberry Pi hardware.
The trained model reached ~75% classification accuracy across all 7 emotion classes.
Worked with teammates to integrate the model's output into the mood-to-music recommendation engine and the Alexa voice layer.
Architecture
Camera (Raspberry Pi) → Face detection → MobileNet CNN (emotion classification)
      → Mood output → Music recommendation engine → Speaker playback
      → Alexa integration → Voice commands
      → Display → Real-time mood visualization
Tech stack
Hardware: Raspberry Pi, camera module, display, speaker
ML/CV: Python, OpenCV, TensorFlow/Keras (MobileNet, transfer learning), FER-2013 dataset
Voice: Amazon Alexa Skills integration
Interface: Web/display UI for mood + recommendation visualization
Results
~75% accuracy classifying 7 emotion categories (happy, sad, angry, fear, disgust, surprise, neutral) using MobileNet with transfer learning on FER-2013.
Deployed and validated on real-time video input on Raspberry Pi hardware.
Publication

Findings co-authored and published in the International Journal of Science and Management Studies (IJSMS), 2024, E-ISSN: 2581-5946.

Team

Varsha K, Divya S R, Ragasree K, Savija J — B.Tech, Artificial Intelligence & Data Science, Velammal Engineering College (Anna University), 2024.

Notes

This repository currently documents the project's design, model approach, and results. Source code will be added as it's cleaned up for public release.

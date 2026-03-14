# AI Generated Image Detection using CLIP and Random Forest

## Overview
This project presents a computer vision pipeline for detecting whether an image is AI-generated or a real photograph. With the rise of generative AI models such as DALL·E, MidJourney, and Stable Diffusion, distinguishing synthetic images from real ones has become increasingly difficult.

The system uses OpenAI's CLIP model to extract high-level image embeddings and a Random Forest classifier to perform binary classification.

## Features
- Detects AI-generated images vs real photographs
- Uses CLIP embeddings (512-dimensional feature vectors)
- Random Forest classifier for efficient prediction
- Data augmentation for improved training
- Confidence score for each prediction
- Interactive Gradio web interface

## Technologies Used
- Python
- OpenAI CLIP
- PyTorch
- Scikit-learn
- Gradio
- OpenCV
- NumPy

## Methodology

1. Image Input  
   Images are collected from both real photographs and AI-generated sources.

2. Data Augmentation  
   Each training image is augmented using:
   - Random horizontal flip
   - Rotation (±25°)
   - Color jitter

3. Feature Extraction  
   The CLIP model extracts 512-dimensional embeddings representing semantic image features.

4. Classification  
   A Random Forest classifier is trained using these embeddings to classify images as:
   - AI Generated
   - Real Photograph

5. Prediction Interface  
   A Gradio-based web interface allows users to upload images and receive predictions along with a confidence score.

## Output
The system provides:
- Predicted Label (AI Generated / Real Photograph)
- Confidence Score

## Applications
- Fake image detection
- Social media verification
- Misinformation prevention
- Digital forensics
- Media authentication

## Future Improvements
- Support for multiple generative models
- Larger dataset training
- Deep learning ensemble models
- Real-time detection for social platforms

SAMPLE OUTPUT:
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/caa6964d-3e04-4617-9de2-bf5fddbce4a0" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/585fb7e1-9b76-4745-b073-8bb43f8d800d" />

# Smart-Class-Room

# 📚 Smart Classroom Attendance & Participation System

An AI-powered smart classroom solution that automatically detects students, recognizes faces, tracks their presence, and monitors hand-raising behavior in real-time using computer vision and deep learning.

## 🎯 Project Overview

This project automates classroom monitoring by analyzing video footage to:
- Detect student faces for **attendance tracking**
- Track individuals across frames
- Recognize **raised hands** using pose estimation
- Generate a CSV report summarizing participation and attendance

## 🧠 Technologies Used

| Technology        | Purpose                                                                 |
|-------------------|-------------------------------------------------------------------------|
| **YOLOv5**         | Person detection from classroom video                                  |
| **Deep SORT**      | Object tracking across frames (maintains consistent student ID)       |
| **InsightFace**    | Face recognition through deep embeddings                              |
| **Keypoint R-CNN** | Pose estimation (detect raised hands using keypoints)                 |
| **OpenCV**         | Video processing and annotation                                       |
| **PyTorch**        | Deep learning framework for models and inference                      |
| **Google Colab**   | Development and testing environment                                    |

# Smart-Class-Room

Here is a complete and professional `README.md` file for your GitHub repository based on the Smart Classroom project:

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

## 🛠️ Setup Instructions

1. Clone the repository:

```bash
git clone https://github.com/your-username/Smart-Classroom.git
cd Smart-Classroom
```

2. Install required dependencies:

```bash
pip install torch torchvision
pip install yolov5
pip install insightface
pip install deep_sort_realtime
pip install onnxruntime
```

> Note: Google Colab users can run all installation steps at the top of the script directly.

3. Place student images inside the `students/` folder. Make sure filenames match student names.

4. Replace the classroom video with your own under the name `classroom_clip.mp4`.

5. Run the script:

```bash
python Smart_Class_Room.py
```

## 📈 Output

* A processed video with:

  * Student names
  * Face recognition boxes
  * Live hand-raise detection
* A `hand_raise_report.csv` file including:

  * Total students
  * Attendance count
  * Number of hand raises per student

## 👏 Acknowledgements

Special thanks to:

* My amazing collaborators 🙌
* Our supportive instructor 🎓
* The hosting training organization 🏢

*(Please replace with actual names in your version)*

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 💡 Future Work

* Real-time dashboard for live classroom analytics
* Integration with Learning Management Systems (LMS)
* Enhanced multi-camera support for larger rooms


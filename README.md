# Face Recognition Attendance System

A real-time face recognition application that automatically marks attendance using computer vision and facial recognition technology.

## 🚀 Features

- **Real-time Face Detection**: Captures video feed and detects faces in real-time
- **Automatic Attendance Tracking**: Records attendance with timestamps in CSV format
- **Multiple Person Recognition**: Can recognize and track multiple individuals
- **User-friendly Interface**: Simple webcam-based interface with visual feedback
- **Efficient Encoding**: Pre-computes face encodings for faster recognition

## 🛠️ Technologies Used

- **OpenCV** - Computer vision and image processing
- **face_recognition** - Facial recognition library built on dlib
- **NumPy** - Numerical computations and array handling
- **Python** - Core programming language

## 📁 Project Structure
PythonProject/
├── AttendenceImages/ # Folder containing reference images for recognition
├── Attendence.csv # Generated attendance records
├── main.py # Main application code
└── README.md # Project documentation


## 🎯 How It Works

1. **Initialization**: Loads reference images from `AttendenceImages/` folder
2. **Encoding**: Pre-computes facial encodings for all reference images
3. **Real-time Processing**:
   - Captures video feed from webcam
   - Detects and encodes faces in each frame
   - Compares with pre-computed encodings
   - Identifies recognized individuals
4. **Attendance Recording**:
   - Records recognized names with timestamps
   - Prevents duplicate entries for the same session
   - Saves data to `Attendence.csv`

## 📊 Output Format

The system generates a CSV file with the following format:
Name,Time
John_Doe,14:30:25
Jane_Smith,14:31:10


## ⚙️ Setup Instructions

### Prerequisites
bash
pip install opencv-python numpy face-recognition

**Usage**
1.Add reference images to AttendenceImages/ folder (named as PersonName.jpg)
2.Run the application
3.Look at the webcam to be recognized
4.Attendance will be automatically recorded in Attendence.csv







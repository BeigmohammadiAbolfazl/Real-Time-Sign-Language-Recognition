# 🤟 Real-Time Sign Language Recognition

A real-time **Sign Language and Hand Gesture Recognition System** developed using **Python, Computer Vision, and Deep Learning**.

The system uses a webcam to detect the user's hand, extract hand landmarks, process the detected gesture, and classify it using a pre-trained **Convolutional Neural Network (CNN)** model.

---

## 📌 Overview

Communication through sign language is an important way for people with hearing or speech impairments to interact with others.

This project aims to provide a computer vision-based solution for recognizing hand gestures in real time. The application captures video from a webcam, detects the hand using **CVZone**, processes the detected hand landmarks, and uses a trained CNN model to predict the corresponding gesture.

The project also includes a graphical user interface for real-time interaction and prediction.

---

## ✨ Features

- 🎥 Real-time webcam-based hand detection
- ✋ Hand landmark detection
- 🔢 Extraction of 21 hand landmark points
- 🧠 CNN-based gesture classification
- ⚡ Real-time prediction
- 🖥️ Graphical User Interface using Tkinter
- 🔊 Text-to-Speech support
- 📊 Custom data collection scripts
- 🧪 Prediction mode with and without GUI
- 🤖 Pre-trained deep learning model

---

## 🏗️ System Architecture

```text
                ┌─────────────────┐
                │     Webcam      │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │   Hand Detection│
                │     CVZone      │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │ Hand Landmarks  │
                │   21 Points     │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │ Image / Feature │
                │   Processing    │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │   CNN Model     │
                │    (Keras)      │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │ Gesture / Sign  │
                │   Prediction    │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │ GUI / Speech    │
                │     Output      │
                └─────────────────┘
```

---

## 🧠 Machine Learning Model

The project uses a **Convolutional Neural Network (CNN)** for gesture classification.

The trained model is provided in:

```text
cnn8grps_rad1_model.h5
```

The model receives the processed representation of the detected hand gesture and predicts the corresponding class.

---

## 📂 Project Structure

```text
Real-Time-Sign-Language-Recognition/
│
├── 📄 final_pred.py
│   └── Main application with graphical interface
│
├── 📄 prediction_wo_gui.py
│   └── Gesture prediction without GUI
│
├── 📄 data_collection_final.py
│   └── Hand gesture data collection
│
├── 📄 data_collection_binary.py
│   └── Binary gesture data collection
│
├── 🧠 cnn8grps_rad1_model.h5
│   └── Pre-trained CNN model
│
├── 🖼️ white.jpg
│   └── Image used during hand landmark processing
│
├── 📄 requirements.txt
│   └── Required Python dependencies
│
├── 📄 README.md
│   └── Project documentation
│
└── 📄 .gitignore
    └── Git ignored files
```

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| 🐍 Python | Core programming language |
| 👁️ OpenCV | Computer vision and webcam processing |
| ✋ CVZone | Hand detection and landmark extraction |
| 🧠 TensorFlow / Keras | CNN model and deep learning |
| 🔢 NumPy | Numerical and array processing |
| 🖥️ Tkinter | Graphical user interface |
| 🔊 Pyttsx3 | Text-to-Speech |
| 🖼️ Pillow | Image processing |

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/Real-Time-Sign-Language-Recognition.git
```

### 2. Navigate to the project directory

```bash
cd Real-Time-Sign-Language-Recognition
```

### 3. Create a virtual environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Application

To run the main application:

```bash
python final_pred.py
```

Make sure that:

- Your webcam is connected.
- Python dependencies are installed.
- The trained model file is located in the project directory.
- The required image files are available.

---

## 📊 Data Collection

The project includes scripts for collecting hand gesture data.

Run:

```bash
python data_collection_final.py
```

or:

```bash
python data_collection_binary.py
```

These scripts can be used to capture and prepare additional hand gesture samples for experimentation and model development.

---

## 🔮 Prediction Without GUI

For running the recognition system without the graphical interface:

```bash
python prediction_wo_gui.py
```

This provides a lightweight prediction pipeline suitable for testing and experimentation.

---

## 🎯 Applications

This type of system can be used as a foundation for:

- Sign language recognition
- Human-computer interaction
- Gesture-based interfaces
- Accessibility applications
- Educational tools
- Computer vision research
- Real-time gesture-controlled systems

---

## 🚀 Future Improvements

Potential improvements include:

- [ ] Support for a larger sign language vocabulary
- [ ] Improved CNN architecture
- [ ] Real-time sentence construction
- [ ] Multi-hand gesture recognition
- [ ] Improved recognition accuracy
- [ ] Support for dynamic gestures
- [ ] Web-based interface
- [ ] Mobile application
- [ ] Transformer-based gesture recognition
- [ ] Real-time translation into natural language

---

## 📈 Project Workflow

```text
Camera Input
     │
     ▼
Hand Detection
     │
     ▼
Landmark Extraction
     │
     ▼
Image Preprocessing
     │
     ▼
CNN Classification
     │
     ▼
Gesture Recognition
     │
     ▼
Text / Speech Output
```

---

## 🔬 Project Type

**Computer Vision · Deep Learning · Machine Learning · Sign Language Recognition · Human-Computer Interaction**

---

## 👨‍💻 Author

**Abolfazl Big Mohammadi**

Computer Science / Software Engineering  
Interested in **Artificial Intelligence, Machine Learning, Computer Vision, and Software Development**.

---

## 📜 License

This project is intended for **educational and research purposes**.

If you use or modify this project, please provide appropriate attribution to the original work.

---

## ⭐ Support

If you find this project useful, consider giving the repository a ⭐ on GitHub.
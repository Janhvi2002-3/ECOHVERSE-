✋ Sign Language to Text Conversion
A Deep Learning project to convert American Sign Language (ASL) to text format using a real-time webcam feed and a custom-trained CNN model.

📁 Project Structure
Documentation Folder – Contains the project report.

Source Code Folder – All Python source files.

Model Folder – Trained CNN model files (.json, .h5).

Pics Folder – Sign language images of all characters.

🔑 Key Project Files and Their Purpose
| File                                       | Description                                                                                                         |
| ------------------------------------------ | ------------------------------------------------------------------------------------------------------------------- |
| `collect-data.py`                          | Used to **create your own dataset** of sign language images for each character.                                     |
| `image_processing.py` & `preprocessing.py` | Converts images to **black & white** and applies **Gaussian blur** for better edge detection and improved accuracy. |
| `train.py`                                 | Contains the code to **train the CNN model**. Outputs `.json` and `.h5` model files.                                |
| `app.py`                                   | Contains the **GUI code built using Tkinter**. It runs the frontend for sign language detection.                    |

🛠️ Steps to Execute the Project
1. Create Your Dataset
Run collect-data.py to capture your own sign language data.

2. Preprocess Images
Run image_processing.py and preprocessing.py to generate black & white, blurred images.

3. Train the Model
Run train.py to train the CNN and generate model.json and model.h5.

4. Launch the GUI
Run app.py to open the frontend window and start real-time sign language to text conversion.

💡 How the Frontend Works
1.The GUI opens via Tkinter.

2.Show the sign language gesture in front of the webcam.

3.The model captures 50 frames and predicts the most frequent character from those.

4.When no hand is detected, the model understands the word is completed.

5.Predicted characters form words, and then full sentences.

📦 Installation Requirements
1. 🐍 Python Version
Python 3.10.12

2. 📚 Required Python Libraries
| Library         | Version  | Purpose                      |
| --------------- | -------- | ---------------------------- |
| `tensorflow`    | 2.11.0   | CNN model (Keras-based)      |
| `opencv-python` | 4.8.0.76 | Webcam and image processing  |
| `mediapipe`     | 0.10.7   | Real-time hand tracking      |
| `numpy`         | 1.23.5   | Numerical operations         |
| `pillow`        | 9.5.0    | Image handling in Tkinter    |
| `scikit-learn`  | 1.2.2    | Confusion matrix, evaluation |
| `matplotlib`    | 3.7.1    | Visualization                |
| `tkinter`       | Built-in | GUI application              |
| `json`          | Built-in | Load model/class files       |
| `h5py`          | 3.8.0    | Load `.h5` model weights     |


3. 💻 Recommended IDE
Visual Studio Code (for best debugging experience)



🗂 Suggested Folder Structure
pgsql
Copy
Edit
Sign-Language-to-Text-Conversion/
│
├── source_code/
│   ├── app.py
│   ├── collect-data.py
│   ├── image_processing.py
│   ├── preprocessing.py
│   ├── train.py
│   ├── model.json
│   ├── model.h5
│   ├── class_labels.json
│
├── test_images/
├── model/
├── pics/
├── documentation/
│   └── project_report.pdf
├── README.md
└── requirements.txt

📌 Final Notes
> This project supports both real-time prediction and custom dataset creation.

> Ideal for building a gesture-based communication system.

> Can be extended to include sentences, numbers, or dynamic gestures.

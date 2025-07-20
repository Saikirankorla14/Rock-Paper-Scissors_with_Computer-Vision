# Rock-Paper-Scissors_with_Computer-Vision

🎯 Project Goal
Build an interactive Rock-Paper-Scissors (RPS) game where a user can play against the computer using hand gestures detected by a webcam. The AI model classifies the user's move using a Convolutional Neural Network (CNN).
🛠️ Tools & Technologies
- OpenCV – for real-time hand gesture detection via webcam
- TensorFlow / Keras – to build and train a CNN for gesture classification
- NumPy / Matplotlib – for preprocessing and visualization
📂 Dataset
A custom or public dataset of hand gestures representing Rock, Paper, and Scissors images. Each image is labeled as one of the three classes. Optionally, you can collect your own using OpenCV.
🏗️ Project Structure

rps-computer-vision/
│
├── data/
│   └── rock/, paper/, scissors/
├── model/
│   └── rps_model.h5
├── app/
│   └── rps_game.py
├── utils/
│   └── preprocess.py
├── train/
│   └── train_model.py
├── README.docx
└── requirements.txt

🧠 Model Architecture
Input: 64x64 or 128x128 RGB images
Layers:
- Conv2D → ReLU → MaxPooling
- Conv2D → ReLU → MaxPooling
- Flatten → Dense → Dropout
- Output Layer: Softmax (3 classes: Rock, Paper, Scissors)
🕹️ How to Play
1. Run the game:
   python app/rps_game.py
2. Show your hand gesture (rock, paper, or scissors) to the webcam
3. The model classifies your move and plays against you in real-time
🔧 Installation Steps
1. Clone the Repository:
   git clone https://github.com/yourusername/rps-computer-vision.git
2. Install Dependencies:
   pip install -r requirements.txt
3. (Optional) Train your model:
   python train/train_model.py
4. Run the Game:
   python app/rps_game.py
✅ Future Improvements
- Add Lizard and Spock to extend RPSLS
- Improve model accuracy using data augmentation
- Add a GUI using Tkinter or PyQt
- Deploy as a web app using Streamlit or Flask

Model Accuracy and Model Loss:
<img width="1189" height="590" alt="Model_accuracy_RPS" src="https://github.com/user-attachments/assets/1457f3d6-1245-4fcf-990f-407f6832d7bc" />




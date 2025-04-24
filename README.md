![background](https://github.com/user-attachments/assets/276f1c2c-6133-4c6c-b56c-861e43cd83dc)# 🗳️ Online Voting System

This is a Python-based **face recognition voting system** where users can vote using their face and Aadhar number. It uses OpenCV for facial recognition, scikit-learn for model training (KNN), and stores votes securely in a CSV file.

## 📁 Project Structure
├── add_faces.py # Register new voters with face data and Aadhar number 
├── give_vote.py # Face recognition + voting interface 
├── background.png # UI background image for the voting interface 
├── requirements.txt # Python dependencies 
├── votes.csv # Stores the final voting data 
└── data/ 
├── faces_data.pkl # Saved facial features 
└── names.pkl # Saved Aadhar numbers linked to faces


## ⚙️ Setup Instructions

1. **Clone the Repository**  
   ```bash
   git clone https://github.com/yourusername/online-voting-system.git
   cd online-voting-system
pip install -r requirements.txt
Enter your Aadhar number and let the camera capture 51 frames.
python add_faces.py
python give_vote.py
The webcam will scan your face. Once recognized, press:
1: BJP
2: CONGRESS
3: AAP
4: NOTA
How It Works
Face Recognition: Captures and processes 50x50 pixel facial images and stores them as flattened NumPy arrays.

Model: K-Nearest Neighbors (KNN) is used to match incoming faces with stored ones.

Voting: Once authenticated, the user can vote only once. All votes are recorded with timestamps in votes.csv.
Features
Face-based authentication using webcam

Aadhar number verification

Ensures one vote per user

Real-time voting interface

Vocal feedback using Windows text-to-speech
his project uses win32com.client (works only on Windows for speech synthesis).

Make sure your webcam is connected and functioning.

The system doesn't support deletion/editing of votes for integrity.






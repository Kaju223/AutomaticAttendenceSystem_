This project automates attendance marking using face recognition with OpenCV. It captures, trains, and recognizes faces to mark attendance in a CSV file.

📌 Features
✅ Face detection using Haar Cascade
✅ Face recognition using LBPH model
✅ Automatic attendance marking in CSV
✅ Identifies unknown faces
✅ Marks absent students

📌 Steps to Run the Project

1️⃣ Create a New Project in PyCharm
Open PyCharm → Click on New Project → Choose a folder.

2️⃣ Download Haar Cascade XML File (For Face Detection)
Download haarcascade_frontalface_default.xml from the link:
🔗 https://github.com/opencv/opencv/blob/master/data/haarcascades/haarcascade_frontalface_default.xml
Move this file into your project folder.


3️⃣ Install Required Libraries
Go to Settings → Python Interpreter → Install:
opencv-python
opencv-contrib-python
numpy
pandas


4️⃣ Create dataset.py File (For Data Collection)
Write the face capture code.
Attach Haar Cascade in the code:
Run dataset.py → Enter the person's name.
System captures 100 images and saves them in the dataset folder.


5️⃣ Create training.py File (For Training)
Run train_model.py → Trains a model using dataset images.
Saves:
trained_model.xml (Face recognition model)
labels.pkl (Label mappings)


6️⃣ Create detection.py File (For Attendance)
Run detection.py → Recognizes faces from a webcam.
Marks attendance in a CSV file (Attendance_YYYY-MM-DD.csv).
Unknown faces are labeled as "Unknown".


7️⃣ Check Attendance File
Open the CSV file to see the attendance records.
✅ Done! 🚀

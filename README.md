# InstaAttend-Attendance-System-Using-Barcode-and-Face-Recognition
Smart Attendance System Using Barcode and Face Recognition
This project is a Smart Attendance System that uses a combination of barcode scanning and face recognition to mark attendance efficiently and accurately. With a user-friendly Tkinter interface, it allows quick barcode-based identification of students and automatically verifies their identity using live facial recognition. Student information, including an image and personal details, is displayed dynamically, and attendance is marked in an Excel file.

Features
Barcode Scanning: Identifies students by scanning barcodes to retrieve their roll numbers.
Automated Student Details Display: Shows student information and image based on the roll number, fetched from a directory.
Face Recognition: Verifies student identity by matching the displayed image with a live face capture.
Attendance Recording: Marks the student's attendance in an Excel file, along with a timestamp.
Tkinter GUI: Provides a simple, interactive interface for easy usage.
Requirements
Python 3.x
OpenCV (cv2)
face_recognition
pyzbar
PIL (Pillow)
openpyxl
Installation
Clone this repository:
bash
Copy code
git clone <repository_link>
Install dependencies:
bash
Copy code
pip install opencv-python face_recognition pyzbar pillow openpyxl
Place student images and details in a PHOTO folder. Images should be named as <roll_number>.png or <roll_number>.jpg, and details should be stored as text files (<roll_number>.doc) inside individual folders named by roll numbers.
Usage
Run the application:
bash
Copy code
python main.py
Click the Scan Barcode button to scan a student's barcode.
Once the barcode is scanned, the system will automatically display the student's image and details and start face recognition.
If the face is matched successfully, attendance is marked in the attendance.xlsx file.
Project Structure
main.py: Main script containing the application code.
PHOTO/: Folder containing student images and text files with details (create individual folders for each roll number).
attendance.xlsx: Excel file where attendance records are stored.
Notes
Ensure that each student has a unique barcode linked to their roll number.
Make sure the camera and lighting conditions are adequate for barcode scanning and facial recognition.

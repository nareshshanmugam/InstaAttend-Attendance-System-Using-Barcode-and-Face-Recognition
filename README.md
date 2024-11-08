# InstaAttend: Smart Attendance System Using Barcode & Face Recognition

**InstaAttend** is a modern, intelligent attendance management system that leverages barcode scanning and live face recognition to automate and streamline attendance marking. This project integrates a user-friendly Tkinter interface, providing a quick and seamless experience for identifying and verifying students. InstaAttend not only retrieves and displays student information dynamically but also marks attendance in an Excel sheet for record-keeping.

---
## Contributors

- **[NareshKanna S](https://www.linkedin.com/in/nareshkanna-shanmugam-a4462a269/)** - Barcode Scanning Module,collabrator
- **[Prasath Raja K](www.linkedin.com/in/prasath-raja-k-5609aa25a)** -  Live Face Recognition and Tkinter UI Integration
- **[Kishore K](https://www.linkedin.com/in/kishore-k-84b8b1269?trk=contact-info)** - Image and Details Retrieval Module
- **[Selvam S](https://www.linkedin.com/in/selvam-s-b3b8a8269/)** - Attendance Marking Module

- **[Karthikeyan](https://github.com/facultyusername)** - Mentor
- **[Subhashri](https://github.com/facultyusername)** - Mentor




## ✨ Key Features

- **🔍 Barcode Scanning**: Quickly identifies students by scanning unique barcodes associated with their roll numbers.
- **📋 Automated Info Display**: Instantly fetches and displays student details, including an image, from a structured directory.
- **🤳 Face Recognition**: Verifies student identity by matching a live capture with the stored image, ensuring authenticity.
- **🕒 Attendance Recording**: Automatically logs attendance in `attendance.xlsx` with precise timestamps for reliable record management.
- **💻 Intuitive Tkinter Interface**: Clean, interactive GUI makes it easy for users to operate the system without extensive technical knowledge.

---

## 🛠️ Requirements

- Python 3.x
- Libraries:
  - **OpenCV** (`opencv-python`) for video and image handling
  - **face_recognition** for face matching
  - **pyzbar** for barcode scanning
  - **Pillow** (`PIL`) for image processing
  - **openpyxl** for Excel file manipulation

## 📥 Installation

1. **Clone the Repository**:
   ```bash
   git clone <repository_link>
   ```

2. **Install Dependencies**:
   ```bash
   pip install opencv-python face_recognition pyzbar pillow openpyxl
   ```

3. **Prepare Data**:
   - Create a `PHOTO/` directory.
   - Store each student’s image as `<roll_number>.png` or `<roll_number>.jpg` in individual subfolders named by roll numbers.
   - Save student details in text files (`<roll_number>.doc`) within their respective folders.

---

## 🚀 Usage

1. **Launch the Application**:
   ```bash
   python main.py
   ```

2. **Scan a Barcode**:
   - Click **📷 Scan Barcode** in the GUI to scan the student’s barcode.
   - The system will automatically:
     - Retrieve the student’s information and display it, including the profile image.
     - Start face recognition to verify the identity.
   
3. **Face Recognition & Attendance Marking**:
   - Upon successful face match, attendance is automatically logged in `attendance.xlsx` with the current timestamp.

---

## 📂 Project Structure

- `main.py`: Main application script containing all functionalities and the Tkinter GUI.
- `PHOTO/`: Directory to store student data:
  - Individual subfolders for each roll number containing:
    - **Image**: `<roll_number>.png` or `<roll_number>.jpg`
    - **Details**: `<roll_number>.doc`
- `attendance.xlsx`: Excel sheet where attendance records are stored.

---

## 📝 Notes

- Ensure that each barcode uniquely identifies a student roll number.
- Optimal lighting and camera positioning will improve barcode scanning and facial recognition accuracy.
  
---

## 🎉 Why InstaAttend?

**InstaAttend** revolutionizes attendance by combining speed with security. With its barcode-driven identification and face verification, you can eliminate proxy attendance and streamline attendance management for classrooms, events, or workplaces. The interface is designed to be intuitive, ensuring ease of use for administrators without sacrificing security or accuracy.


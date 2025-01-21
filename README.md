# Attendance-Manager-System

# **Attendance System using Face Recognition**  

This project implements an automated attendance system using face recognition. It captures, trains, and recognizes faces to mark attendance in real time.  

---

## **Features**  
- **Face Detection and Recognition**: Detects and recognizes faces in real-time using OpenCV.  
- **CSV Attendance Export**: Attendance records are stored in a CSV file.  
- **User-Friendly GUI**: Simple interface for easy navigation.  
- **Customizable and Expandable**: Can be enhanced with additional features like email notifications or database integration.  

---

## **Installation Instructions**  

### **Prerequisites**  
Ensure you have the following:  
- Python 3.8 or higher installed on your system.  
- Required Python libraries:  
  - `opencv-python`  
  - `numpy`  
  - `pandas`  
  - `Pillow`  
  - `pyttsx3`  

### **Steps to Install**  
1. Clone the repository or download the ZIP file:  
   ```bash  
   git clone <repository_url>  
   cd attendance-system  
   ```  

2. Install the required Python libraries:  
   ```bash  
   pip install -r requirements.txt  
   ```  

3. (Optional) If you plan to create an executable using PyInstaller, install it:  
   ```bash  
   pip install pyinstaller  
   ```  

---

## **How to Use the Project**  

### **Option 1: Run Directly Using Python**  
1. Open a terminal or command prompt in the project directory.  
2. Run the Python script:  
   ```bash  
   python attendance_system.py  
   ```  
3. The GUI will open. Follow the steps in the application to:  
   - **Capture Images**: Enter the user ID and name, then click "Capture Images." Ensure your face is visible for clear image capture.  
   - **Train the Model**: Click "Train Model" to train the system on the captured images.  
   - **Mark Attendance**: Click "Mark Attendance" to start face recognition and mark attendance.  

4. View the `attendance.csv` file in the project directory to see the recorded attendance.  

---

### **Option 2: Run as a Standalone Executable**  
1. Create an executable for the project using PyInstaller:  
   ```bash  
   pyinstaller --onefile --windowed attendance_system.py  
   ```  
2. The executable will be located in the `dist` folder.  
3. Navigate to the `dist` folder and double-click `attendance_system.exe` to run the program without needing Python.  

---

## **File Structure**  
- `attendance_system.py`: Main application file.  
- `haarcascade_frontalface_default.xml`: Pre-trained Haar Cascade model for face detection.  
- `TrainingImage/`: Folder to store captured images for training.  
- `TrainingImageLabel/`: Folder to store the trained model data.  
- `attendance.csv`: Attendance record stored in CSV format.  

---

## **Troubleshooting**  
1. If PyInstaller is not recognized, use this command:  
   ```bash  
   python -m PyInstaller --onefile --windowed attendance_system.py  
   ```  
2. Ensure all libraries are installed. You can reinstall them using:  
   ```bash  
   pip install -r requirements.txt  
   ```  
3. If the face detection accuracy is low, ensure proper lighting and clear visibility of the face during image capture.  

---

## **Future Enhancements**  
- Add email notifications for attendance summaries.  
- Store attendance records in a database.  
- Implement advanced face recognition models like DeepFace for improved accuracy.  

---

## **License**  
This project is open-source and distributed under the [MIT License](LICENSE).  

--- 

# Face-Recognition-Based-Slot-Wise-Attendance-Marking-System

The Face Recognition Based Slot Wise Attendance Marking System is a Python project that utilizes the OpenCV and face_recognition libraries to perform real-time face recognition from webcam feeds. The system can be used to mark attendance of students by comparing their faces with pre-registered images.

# Requirements
    Python 3.x
    OpenCV
    face_recognition
    Numpy

# Getting Started

1. Clone or download the project to your local machine.
2. Make sure you have Python 3.x installed.
3. Install the required dependencies by running:
    3.1  pip install numpy
    3.2  pip install opencv-python
    3.3  pip install face_recognition
4. Create a new folder(name it on your own) for this project such that, inside the current folder 
   create a new folder to add student images. As we are dealing with attendance of students 
   enrolled in different slots make sure to create separate folder for each slot to store student images.

   Path for reference:

                         Attendance --> Student_Images
                                        |
                                        --> A1_Slot_Images
                                        --> A2_Slot_Images
                                        --> B1_Slot_Images

5. Now create a csv file for each slot and save them in Attendance folder.

*NOTE*: Make sure that the downloaded code, student images and csv files all are at one place.
   
# Usage

1. Run the Face_Recognition.py script.
2. The webcam will open, and the system will try to recognize faces in real-time.
3. When a recognized face is detected, the system will mark the attendance of the corresponding 
   student for the current time slot.

 # Customizing Time Slots

 The attendance slots and their corresponding start and end times can be customized. Modify the 
 attendance_slots dictionary in the script to define your desired time slots.

 # Exported Attendance Records

 Attendance records for each time slot will be saved in separate CSV files named as 
 <time_slot>_Attendance.csv, containing the following columns:

    Student Name: Name of the recognized student.
    Registration Number: Unique identifier for the student.
    Time: Time of attendance marked in 12-hour format.
    Date: Date when the attendance was marked.
    Time Slot: The specific time slot for which the attendance was recorded.

*NOTE*: The face recognition accuracy may vary depending on the quality of student images used 
        for registration and real-time webcam lighting conditions.

# Troubleshooting
If you encounter any issues or need further assistance, feel free to contact the project owner or open an issue on the project's GitHub repository.

# Acknowledgments

The Face Recognition Based Attendance System is inspired by various open-source projects and tutorials available in the computer vision and machine learning community. Special thanks to the developers of OpenCV and face_recognition for their excellent libraries.

# Project Overview: Real-Time Face Recognition and Greeting System

This project involves creating an advanced face recognition and greeting system, utilizing computer vision technologies such as OpenCV, DeepFace, and TensorFlow. The integration with hardware like the Raspberry Pi ensures precise real-time identification of individuals from a predefined database, followed by a personalized greeting. The system is intended for use in various environments, including offices, hospitals, and public spaces, with applications in personalized interactions, security, and attendance monitoring.

## Initial Development Phase

- **Face Detection :-** Employed OpenCV's `haarcascade_frontalface_default.xml` to detect human faces.

- **Live Footage Visualization :-** Used Matplotlib to display live footage.

- **Model Training :-** Applied K-Nearest Neighbors (KNN) and Convolutional Neural Network (CNN) algorithms for real-time face recognition.

- **Hardware Setup :-** Set up a Raspberry Pi module to handle processing, training, and model deployment. Supported by the Pi Camera Module 2 for image capture.

## Optimization Phase

- **Model Enhancement :-** Shifted to model training with the Random Forest algorithm to reduce lag.

- **Image Preprocessing :-** Utilized the Pillow library for image preprocessing to improve face detection speed and streamline real-time processing.

## User Interface Development

- **UI Integration :-** Created a user-friendly interface with Flask acting as the backend server.

- **Frontend Tools :-** Employed HTML, CSS, Bootstrap, and JavaScript to build an interactive frontend that shows real-time face detection results.

## Advanced Model and Hardware Integration

- **Advanced Model Integration :-** Integrated DeepFace into the model, achieving approximately 88% accuracy with a larger database.

- **Hardware Considerations :-** Considered alternatives such as the Grove Vision AI V2, which features an ARM Cortex-M55 processor and ARM Ethos-U55 NPU, and the Xiao ESP32S3 for wireless communication, due to the limitations of the Raspberry Pi’s hardware.
- **Cost-Effective Solutions :-** Assessed the Realtek AMB82-Mini 8-in-1 SoC, which provides embedded AI capabilities and efficient high-resolution processing up to 2K at 0.4 TOPs, ensuring cost-effective implementation.

## Directory Structure

- **img folder:** Contains processed images of individuals, correctly labeled with timestamps, for model training.
- **peoples folder:** Stores images directly uploaded by users for future reference, with deletion managed by removing references in this folder.
- **templates folder:** Contains HTML, CSS, and JavaScript files for building the user interface.
- **uploads folder:** Holds images during the processing stage.
- **app.py:** The backend file hosting the user interface. Run this file to start the application on localhost:5000, which can be updated once deployed with a domain.
- **final_model_rf.py:** Contains the ML model for real-time face detection.
- **face_extractor.ipynb:** Includes code for the DeepFace model.

## Running the Server

To upload a picture and run the server, navigate to the directory containing app.py and execute the following command in the terminal:
python3 app.py

## Project Overview
This project presents an advanced face recognition and greeting system using OpenCV, DeepFace, and TensorFlow, integrated with the Raspberry Pi. It is designed to accurately identify individuals from a database in real-time and greet them by name. The system is well-suited for deployment in offices, hospitals, and public spaces, offering applications in personalized interactions, security, and attendance tracking.
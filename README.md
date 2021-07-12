# Drowsiness-Detection
A Neural Network model that detects whether a person is drowsy or not by capturing the Image part and sending it to the model.
# What is Drowsiness - Detection ?
 It is a safety technology that detects the drowsiness of the drivers while driving the vechiles and prevents the accidents. The objective of this project is detect the face of the driver(with **Open CV**) and identify whether eyes are closed or not (Through **Neural network model**) and alert the driver through an alarm if driver closes eyes for more than certain threshold seconds.
 
 
 # Flow of Drowsiness-Detection System 
 In this project we will be using **Open CV** to gather images from the webcam and send the collected frames to the deep learning model to classify whether eyes are closed or not.
 The steps involved in this project are as follows
 1. Take the image from webcam as input
 2. Detect the face from the image and create Region of Intrest(**ROI**)
 3. Detect the eyes from the face and send it to the classifier
 4. Classifier will identify whether eyes are closed or not
 5. Calculate the score based on the result of classifier
 6. If score is more than the threshold the alarm gets activated 

# Project Requirements
This project requires webcam to take images and to execute this project python(latest version) should be installed on your system and with pip you can install the following packages
1. **Open CV**      - `pip install opencv-python `(to detect face and eyes)
2. **TensorFlow**   - `pip install tensorflow `(keras uses tensorflow)
3. **Keras**        - `pip install keras`(to build classification model)
4. **Pygame**       - `pip install pygame`(to play alarm sound)

# Files description of this project
* **main.py** - the starting point of the project execution
* **model.py** - the deep learning model architecture of the classfier
* **binary_cnn.h5** - the trained model file
* **haar cascade files** - files for opencv to detect face and eyes
* **alarm** - wav file for alarm

# Project Execution
To execute this project open command prompt and the type command `python main.py` before executing this command make sure you have installed all required packages. It is better to create python environmet to avoid dependencies errors. If python environment is created then exeute above command after activating the environment.

It take few seconds to open the webcam and start detection

** Example output **

**When Eyes closed**

![Screenshot (45)](https://user-images.githubusercontent.com/69287549/125242503-6b0b1a80-e30a-11eb-808b-f6e3fe128b99.png)

**When Eyes Opened**
![Screenshot (47)](https://user-images.githubusercontent.com/69287549/125242801-c806d080-e30a-11eb-8754-e72a2ac39bea.png)








 

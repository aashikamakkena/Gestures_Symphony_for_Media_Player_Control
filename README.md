# Gestures_Symphony_for_Media_Player_Control

## A Web Application to control media player using Hand gestures (Using Streamlit)

In response to the growing need for efficient interactions with technology, this project explores gesture recognition for controlling media players using a device's webcam to track and interpret hand movements. By identifying seven specific gestures, this innovative system enables users to control various functions of media players solely through their device's camera. This approach leverages Deep Learning algorithms, eliminating the necessity for additional hardware and transforming how users interact with technology. Gesture recognition not only facilitates hands-free media control but also enables touchless device navigation and seamless smart home management. Additionally, this technology holds promise for aiding visually impaired individuals in effectively controlling media players.

The proposed system can control the media player from a distance using hand gestures.

1. Data Acquisition and Preprocessing Phase:
We collect image data through a webcam in the form of a video stream. This video stream is broken down into individual frames, allowing for the manipulation of discrete images. These frames are then processed using OpenCV, a computer vision library, to convert them into black and white images and are organized and stored in specific directories.

2. Model Building and Feature Extraction:
A Convolutional Neural Network (CNN) model is constructed using Keras, a high-level neural networks API. The ImageDataGenerator class from Keras is employed to preprocess the images stored in the directories, allowing for the extraction of essential features required
for training the model. This step prepares the dataset for the training phase where the CNN model learns to recognize patterns and features within the images.

3. Classification and Prediction:
The compiled model is evaluated for its accuracy using a separate set of test data to assess its performance in recognizing and classifying hand gestures. Incoming gestures are classified into specific predefined classes. This classification enables
the system to interpret gestures made by users and associate them with predefined actions or commands.

4. Integrating Keyboard Controls:
Integrate the recognized gestures with control functions using the Pyautogui library where each detected gesture corresponds to a predefined function, allowing users to control media player actions. To show the functionality and accessibility
of the system, a web application is deployed. This application includes all necessary project files and is made available via Streamlit sharing.

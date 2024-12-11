# 🚗 Vehicle Detection and Counting Using OpenCV and Haar Cascades

Welcome to the __Vehicle Detection__ and Counting project! This project uses __OpenCV__ and __Haar Cascades__ to detect and count vehicles (cars and buses) 
in both images and videos. The primary goal is to detect vehicles in real-time or from recorded footage, highlight them with rectangles, 
and count how many vehicles are present in each frame.

This solution is built using machine learning-based object detection methods (Haar cascades) and image preprocessing techniques to accurately
identify vehicles in various environments.

# 🚀 Features:

* Vehicle Detection: Uses pre-trained Haar Cascade Classifiers (cars.xml, Bus_front.xml) to detect vehicles (cars and buses).
* Image Preprocessing: Enhances detection accuracy by resizing, grayscale conversion, Gaussian blur, and dilation.
* Real-Time Vehicle Counting: Counts and displays the number of detected vehicles.
* Video Processing: Processes each video frame, detects vehicles, and outputs a video with vehicle counts and rectangles around detected vehicles.

# 🛠 Technologies Used:

OpenCV: A powerful library for computer vision tasks.
Haar Cascade Classifiers: Machine learning-based method to detect objects in images.
Python: The language used for this project.

# 📷 How it Works:

1. __Image Preprocessing:__
Resize the input image to a fixed size for consistency.
Convert the image to grayscale to simplify processing.
Apply Gaussian blur to reduce noise and improve detection.
Perform dilation and morphological transformations to enhance detection regions.

2. __Object Detection:__
Load pre-trained Haar cascade classifiers for car and bus detection.
Detect vehicles by running detectMultiScale() on the preprocessed image.
Draw rectangles around detected vehicles using cv2.rectangle().

3.__Counting Vehicles:__
Count the number of detected vehicles and display the count on the image/video.

4. __Video Processing:__
Read video frames, process each one, and save the resulting video with detected vehicles and their count.

# 📥 Installation:

1. Clone the repository:

git clone https://github.com/yourusername/vehicle-detection-and-counting.git
cd vehicle-detection-and-counting

2. Install the required libraries:
pip install opencv-python

3. Download the Haar Cascade files (cars.xml and Bus_front.xml), or you can use the pre-trained classifiers available in the repository.

# ⚙ Usage:

1. ___Single Image Detection:___
Place your image in the repository directory.
Run the Python script to detect and count vehicles in the image.

python detect_vehicles_in_image.py

The processed image with detected vehicles and count will be saved or displayed.

2. ___Video Detection:___
Place your video in the repository directory.
Run the Python script to detect and count vehicles in each frame.

python detect_vehicles_in_video.py

The processed video with detected vehicles and count will be saved as an output video file.

# 🔧 Customizing the Classifiers:

You can train your own Haar Cascade Classifiers if needed. OpenCV provides tools to create custom classifiers for different types of vehicles or objects. 
Refer to the OpenCV Cascade Classifier Training documentation for more details.

# 🌟 Example:

Input Image:

Processed Output:

Detected vehicles will be highlighted with rectangles and the count displayed.

# Happy coding and happy vehicle detecting! 🚙

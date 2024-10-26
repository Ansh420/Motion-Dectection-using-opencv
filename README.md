
![images](https://github.com/user-attachments/assets/202b93de-8bdd-4861-bc6a-9c5a6c25ee6e)
# Motion-Dectection-using-opencv
This Python script demonstrates how to detect motion in real-time using OpenCV. The script captures frames from the default webcam, processes them to detect motion, and draws bounding boxes around the detected moving objects.

## Requirements
- **OpenCV**: Install OpenCV using pip install opencv-python
- **NumPy**: Install NumPy using pip install numpy

## Usage
**Clone the Repository:**

git clone **https://github.com/Ansh420/motion-detection-opencv.git**

**Run the Script:**

python motion_detection.py

![sddefault](https://github.com/user-attachments/assets/52794db1-27b8-40b8-b802-904096ba953d)

# **Explanation**
The script follows these steps:

- **Initialize Video Capture**: Creates a VideoCapture object to capture frames from the default webcam.
- **Read Frames**: Continuously reads frames from the webcam.
- **Convert to Grayscale**: Converts the captured frames to grayscale for faster processing.
- **Blur**: Applies Gaussian blurring to reduce noise in the image.
- **Create Background Subtractor**: Initializes a background subtractor algorithm **(e.g., MOG2)** to learn the background scene.
- **Detect Motion**: Uses the background subtractor to detect moving objects in the current frame.
- **Find Contours**: Finds contours in the detected motion mask.
- **Draw Bounding Boxes**: Draws bounding boxes around the detected contours.
- **Display Frame**: Displays the processed frame with the bounding boxes.
# Customization
- **Background Subtractor**: Experiment with different background subtractor algorithms (e.g., KNN, GMG) to find the best performance for your use case.
- **Thresholding**: Adjust the threshold parameter in the background subtractor to control the sensitivity of motion detection.
- **Contour Filtering**: Implement additional filtering techniques (e.g., area, shape) to refine the detected contours.
- **Multiple Cameras**: Modify the script to capture frames from multiple webcams.

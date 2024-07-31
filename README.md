# Object-Detection-AI
It is designed to perform object detection on a video using a pre-trained MobileNet SSD model in Caffe format. It tracks the entry times of specific objects (person and dog) and saves these times to a CSV file.

Step 1: Download the Model Files: Download the MobileNet-SSD model files manually.
deploy.prototxt from https://github.com/chuanqi305/MobileNet-SSD/blob/master/deploy.prototxt
mobilenet_iter_73000.caffemodel from https://github.com/chuanqi305/MobileNet-SSD/blob/master/mobilenet_iter_73000.caffemodel
Step 2:Place the Files in the Same Directory: Ensure both files are placed in a directory that is accessible from the Jupyter Notebook.
Step 3:Update the Paths in the Code: Update the code to point to the correct paths where these files are stored.

Steps to Run the Code:
Ensure you have the required Python packages installed. If not, you can install them using:- pip install opencv-python opencv-python-headless numpy
Model Files: Make sure you have the deploy.prototxt and mobilenet_iter_73000.caffemodel files in the specified directory (C:/Users/Asus/).
Run the Code: Execute the code in your Jupyter Notebook or Python environment.

Explanation
1) Model Loading: The MobileNet SSD model is loaded using the cv2.dnn.readNetFromCaffe method.
2) Video Processing: The video is processed frame by frame.
3) Object Detection: Each frame is analyzed to detect objects, focusing on the "person" and "dog" label.
4) Entry Time Calculation: The entry time of the first detected person and dog are recorded.
5) CSV Output: The detected entry time is saved in a CSV file.
This code should detect the entry time of the man as well as the dog in the provided video and save the result to a CSV file.

Here's a brief overview of the key steps:
1) Model Loading: You load the MobileNet SSD model using the cv2.dnn.readNetFromCaffe function.
2) Class Labels: You define the class labels that the MobileNet SSD model is trained to detect.
3) Video Capture: You load the video using cv2.VideoCapture.
4) Object Detection Loop: The loop reads each frame, processes it to detect objects, and checks if a person or dog appears in the frame.
5) Non-Maximum Suppression: You apply Non-Maximum Suppression (NMS) to reduce overlapping bounding boxes for the same object.
6) Entry Time Calculation: You calculate and store the entry time for the detected objects.
7) Visualization: Detected objects are highlighted with bounding boxes and labeled.
8) CSV Writing: The entry times for the detected objects are written to a CSV file.

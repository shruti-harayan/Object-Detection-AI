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

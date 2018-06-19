# video-object-detection-tensorflow
An Easy to install application of tensorflow object detection, using opencv. This is an implementation of the tensorflow object_detection research. 
Windows Support only 
### Requirements
A web camera, or a USB web camera.
## Anaconda Image
Preferably anaconda python 3.6 version: https://www.anaconda.com/download/#windows
This image is not optional, the library will not have the proper dependencies without it.
<br>
Navigate to where ```environment.yml``` is located and run:
```
conda env create -f environment.yml #Should supply proper python image
```
After creating the environment, anaconda should automatically mount the new environment. From here follow the installation:
## Installation 
```
pip install opencv-python
pip install matplotlib
pip install image
pip install Cython
#Warning this will change your tensorflow version
pip install --ignore-installed --upgrade tensorflow==1.5
```
Or for GPU:
```
pip install --ignore-installed --upgrade tensorflow-gpu
```
## Running
Remember to navigate into the correct file system first. 
```
python main.py
```
### Multiple Cameras
Sometimes opencv gets confused, if multiple cameras are connected. If opencv is selecting the wrong camera, or is throwing errors, change ```cap = cv2.VideoCapture(0)``` to ```cap = cv2.VideoCapture(1)``` in ```main.py```.

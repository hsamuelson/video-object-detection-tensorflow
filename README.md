# video-object-detection-tensorflow
![alt text](https://cdn-images-1.medium.com/max/1600/1*IWWOPIYLqqF9i_gXPmBk3g.png)

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
conda activate tf15 #To activate the enviorment
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
pip install --ignore-installed --upgrade tensorflow-gpu==1.5

```
It is important to note that the gpu version requires additional requirements see: https://www.tensorflow.org/install/install_windows
## Running
Remember to navigate into the correct file system first. 
```
python main.py
```
### Multiple Cameras
Sometimes opencv gets confused, if multiple cameras are connected. If opencv is selecting the wrong camera, or is throwing errors, change ```cap = cv2.VideoCapture(0)``` to ```cap = cv2.VideoCapture(1)``` in ```main.py```.

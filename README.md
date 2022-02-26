# SmartBrain




An open-source python library built to empower developers to build applications and systems with self-contained Deep Learning capabilities using simple
 and few lines of code.
 
  
 
## ---------------------------------------------------
## SmartBrain will switch to PyTorch backend .
## ---------------------------------------------------
 
![](logo1.png)

An **DeepQuest AI** (A Brand of AI Commons Global Limited)  project [deepquestai.com](https://deepquestai.com).

Developed and Maintained by [Moses Olafenwa](https://twitter.com/OlafenwaMoses) and [John Olafenwa](https://twitter.com/johnolafenwa), brothers, creators of [TorchFusion](https://github.com/johnolafenwa/TorchFusion), Authors of [Introduction to Deep Computer Vision](https://john.aicommons.science/deepvision) and creators of [DeepStack AI Server](https://deepstack.cc).

---

Built with simplicity in mind, **SmartBrain** 
    supports a list of state-of-the-art Machine Learning algorithms for image prediction, custom image prediction, object detection, video detection, video object tracking
    and image predictions trainings. **SmartBrain** currently supports image prediction and training using 4 different Machine Learning algorithms 
    trained on the ImageNet-1000 dataset. **SmartBrain** also supports object detection, video detection and object tracking  using RetinaNet, YOLOv3 and TinyYOLOv3 trained on COCO dataset. Finally, **SmartBrain** allows you to train custom models for performing detection and recognition of new objects. 
   
Eventually, **SmartBrain** will provide support for a wider
    and more specialized aspects of Computer Vision including and not limited to image 
    recognition in special environments and special fields.


**New Release : ImageAI 2.1.6**

What's new:

- **Support Tensorflow 2.4.0** 
- **SqueezeNet replaced with MobileNetV2** 
- **Added TF 2.x compatible pre-trained models for ResNet recognition and RetinaNet detection**
- **Deprecates '.predictImage()' function for '.classifyImage()'**
- **Renames Model types as below:**
    - ResNet >> ResNet50
    - DenseNet >> DenseNet121
- 


### TABLE OF CONTENTS
- <a href="#dependencies" > :white_square_button: Dependencies</a>
- <a href="#installation" > :white_square_button: Installation</a>
- <a href="#prediction" > :white_square_button: Image Prediction</a>
- <a href="#detection" > :white_square_button: Object Detection</a><br>
- <a href="#videodetection" > :white_square_button: Video Object Detection, Tracking & Analysis</a>
- <a href="#customtraining" > :white_square_button: Custom Model Training</a>
- <a href="#customprediction" > :white_square_button: Custom Image Prediction</a>
- <a href="#customdetectiontraining" > :white_square_button: Custom Detection Model Training</a>
- <a href="#customdetection" > :white_square_button: Custom Object Detection</a>
- <a href="#customvideodetection" > :white_square_button: Custom Video Object Detection & Analysis</a>
- <a href="#documentation" > :white_square_button: Documentation</a>
- <a href="#sample" > :white_square_button: Projects Built on ImageAI</a>
- <a href="#real-time-and-high-performance-implementation" > :white_square_button: High Performance Implementation</a>
- <a href="#recommendation" > :white_square_button: AI Practice Recommendations</a>
- <a href="#contact" > :white_square_button: Contact Developers</a>
- <a href="#citation" > :white_square_button: Citation</a>
- <a href="#sponsors" > :white_square_button: Sponsors</a>
- <a href="#contributors" > :white_square_button: Contributors</a>
- <a href="#ref" > :white_square_button: References</a>



### Dependencies
<div id="dependencies"></div>

To use **SmartBrain** in your application developments, you must have installed the following 
 dependencies before you install **SmartBrain** : 
 
 - Python 3.7.6
 - Tensorflow 2.4.0
 - OpenCV 
 - Keras 2.4.3 

You can install all the dependencies by running the commands below 

**Tensorflow**
```bash
pip install tensorflow==2.4.0
```

or **Tensorflow GPU** if you have NVIDIA GPU with CUDA and cuDNN installed.
```bash
pip install tensorflow-gpu==2.4.0
```

**Other Dependencies**
```bash
pip install keras==2.4.3 numpy==1.19.3 pillow==7.0.0 scipy==1.4.1 h5py==2.10.0 matplotlib==3.3.2 opencv-python keras-resnet==0.2.0
```

### Installation
<div id="installation"></div>
 
To install SmartBrain, run the python installation instruction below in the command line:

```bash
pip install smartbrain --upgrade
```

### Image Prediction
<div id="prediction"></div>

![](./data-images/1.jpg)
 
```
convertible : 52.459555864334106
sports_car : 37.61284649372101
pickup : 3.1751200556755066
car_wheel : 1.817505806684494
minivan : 1.7487050965428352
```

**SmartBrain** provides 4 different algorithms and model types to perform image prediction, trained on the ImageNet-1000 dataset.
The 4 algorithms provided for image prediction include **MobileNetV2**, **ResNet50**, **InceptionV3** and **DenseNet121**. 

Click the link below to see the full sample codes, explanations and best practices guide.

[>>> Tutorial & Guide](imageai/Classification/README.md)


### Object Detection
<div id="detection"></div>

![Input Image](./data-images/image2.jpg)
![Output Image](./data-images/image2new.jpg)

```
person : 91.946941614151
--------------------------------
person : 73.61021637916565
--------------------------------
laptop : 90.24320840835571
--------------------------------
laptop : 73.6881673336029
--------------------------------
laptop : 95.16398310661316
--------------------------------
person : 87.10319399833679
--------------------------------
```

**SmartBrain** provides very convenient and powerful methods to perform object detection on images and extract each object from the image.
The object detection class provides support for RetinaNet, YOLOv3 and TinyYOLOv3, with options to adjust for state of the art performance or real time processing.

Click the link below to see the full sample codes, explanations and best practices guide.


[>>> Tutorial & Guide](imageai/Detection/README.md)


### Video Object Detection and Tracking
<div id="videodetection"></div>

**Video Object Detection & Analysis**

_Below is a snapshot of a video with objects detected._

![](./data-images/video1.jpg)
          
**Video Custom Object Detection (Object Tracking)**

_Below is a snapshot of a video with only person, bicycle and motorcyle detected._

![](./data-images/video2.jpg)

**Video Analysis Visualization**

_Below is a visualization of video analysis returned by **SmartBrain** into a 'per_second' function._

![](./data-images/video_analysis_visualization.jpg)

**SmartBrain** provides very convenient and powerful methods to perform object detection in videos and track specific object(s).
The video object detection class provided only supports  the current state-of-the-art RetinaNet, but with options to adjust for state of the art performance or real time processing.
Click the link to see the full videos, sample codes, explanations and best practices guide.


[>>> Tutorial & Guide](imageai/Detection/VIDEO.md)


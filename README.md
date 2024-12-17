# Object Detection with YOLOv3 in Google Colab

This project demonstrates how to use the YOLOv3 (You Only Look Once) object detection model to detect objects in images using Google Colab. The model is pre-trained on the COCO dataset, allowing it to detect 80 different object classes. The implementation includes capturing images through a webcam and performing real-time object detection in Google Colab.

---

## Requirements

Before running the notebook, ensure you have the necessary Python libraries and YOLOv3 files.

### Python Libraries:
- `opencv-python-headless`: For image processing and handling YOLO model.
- `matplotlib`: For displaying images.

Install the libraries using:

```
bash
!pip install opencv-python-headless
!pip install matplotlib
```

#### The following files are necessary for object detection:

yolov3.weights: The pre-trained weights for YOLOv3.
yolov3.cfg: The configuration file for YOLOv3.
coco.names: A file containing the 80 class labels for object detection.

Download these files using:

```
!wget https://pjreddie.com/media/files/yolov3.weights
!wget https://raw.githubusercontent.com/pjreddie/darknet/master/cfg/yolov3.cfg
!wget https://raw.githubusercontent.com/pjreddie/darknet/master/data/coco.names
```

#### How to Use
Install Dependencies:

Run the cell to install the necessary libraries (opencv-python-headless and matplotlib).
Download YOLOv3 Files:

Download the yolov3.weights, yolov3.cfg, and coco.names files to your Colab environment.
Capture Image from Webcam:

Use the provided take_photo() function to capture an image from your webcam. The function will return the captured image and save it as photo.jpg.

#### Run Object Detection:

Once an image is captured, YOLOv3 will perform object detection on the image. The model identifies objects in the image and draws bounding boxes around them.

#### View Results:

The processed image with bounding boxes around detected objects will be displayed. The image is saved as photo_detected.jpg for later use.

#### Example Output
Upon successful execution, you should see the captured image with bounding boxes drawn around detected objects. Each bounding box is labeled with the object’s class name and a confidence score.

![image](https://github.com/user-attachments/assets/526a36de-1edb-4ee0-82b7-7598b8628248)


### Acknowledgements:
YOLOv3 model and weights
COCO dataset


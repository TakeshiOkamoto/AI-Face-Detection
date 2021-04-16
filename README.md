# AI-Face-Detection

## Environment
Python 3.6  
TensorFlow 1.15.5  
TensorFlow 2.4.0  
tf-nightly 2.6.0 (TensorFlow 2.6.0)  
  
It should work with other versions as well.  
  
## Function  
Detect the face from the image. It also supports multiple faces.  
  
## Example of use
<img src="https://github.com/TakeshiOkamoto/AI-Face-Detection/blob/main/images/result1.jpg">
  
<img src="https://github.com/TakeshiOkamoto/AI-Face-Detection/blob/main/images/result2.jpg">
  
<img src="https://github.com/TakeshiOkamoto/AI-Face-Detection/blob/main/images/result3.jpg">

## How to use  
See object_detection_tutorial.ipynb (Jupyter notebook).  
Adjust the value of detection_scores according to your environment.  
(0.01 to 0.99, default 0.10)  

## About english  
sorry,  English Can understand only 3-year-old level.  
  
## Accuracy, speed
Since I am Japanese, it seems that there were many Japanese in the training images, but the faces of people all over the world can also be detected.  
  
The accuracy is moderate. The processing time can be shortened by reducing the image size.  
  
## About TensorFlow Lite  
It cannot be executed with tf.lite (tflite file) with TensorFlow 2.4.0, but it works with tf-nightly 2.6.0 (development version).  
  
## About face.pb  
Used "ssd_mobilenet_v1_coco".  
  
## Background  
It was created in 2018 with TensorFlow 1.9.0.  
I think that the training image was about 3000-5000 and the labeling work was done manually.  
  
I stopped learning artificial intelligence when I migrated Ubuntu (GeForce GTX 1080 Ti 11GB) to Windows after entering university.  
When I resumed learning artificial intelligence in April 2021, the training / evaluation images and related source code were lost, leaving only frozen_inference_graph.pb (face.pb).  
  
That's why I made it public.  

# ROI-Selection

We can detect 20 objects in images (+1 for the background class), including airplanes, bicycles, birds, boats, bottles, buses, cars, cats, chairs, cows, dining tables, dogs, horses, motorbikes, people, potted plants, sheep, sofas, trains, and tv monitors.

We will use the MobileNet SSD + deep neural network (dnn) module in OpenCV to build our object detector. MobileNet is a neural network used for classification and recognition. SSD is framework used to realize the multibox detector.

Command for running and testing the model: 
python deep_learning_object_detection.py \
	--prototxt MobileNetSSD_deploy.prototxt.txt \
	--model MobileNetSSD_deploy.caffemodel --image images/example_01.jpeg 
  
 In Image directory, store the input images that you want to test.
 1. After firing this commnad, different objects present in the image will be detected and classified with corresponding bounding box around it. The recognised object's class is one of the 20 classes mentioned above.
 2. After this,select the region according to your requirement,and after hitting enter,you will get that particular box of selected region.
 3. Press Esc button to close all the current imgaes and to try another input.

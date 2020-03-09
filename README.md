# ROI-Selection

We can detect 20 objects in images (+1 for the background class), including airplanes, bicycles, birds, boats, bottles, buses, cars, cats, chairs, cows, dining tables, dogs, horses, motorbikes, people, potted plants, sheep, sofas, trains, and tv monitors.

We will use the MobileNet SSD + deep neural network (dnn) module in OpenCV to build our object detector. MobileNet is a neural network used for classification and recognition. SSD is framework used to realize the multibox detector.

Command for running and testing the model: 
python deep_learning_object_detection.py \
	--prototxt MobileNetSSD_deploy.prototxt.txt \
	--model MobileNetSSD_deploy.caffemodel --image images/example_05.jpg 
  
 In Image directory, store the input images that you want to test.
 1. After firing this commnad, different objects present in the image will be detected and classified with corresponding bounding box around it. The recognised object's class is one of the 20 classes mentioned above.
 2. After this,select the region according to your requirement,and after hitting enter,you will get that particular box of selected region.
 3. Press Esc button to close all the current imgaes and to try another input.

MobileNet Citation:
@misc{howard2017mobilenets,
    title={MobileNets: Efficient Convolutional Neural Networks for Mobile Vision Applications},
    author={Andrew G. Howard and Menglong Zhu and Bo Chen and Dmitry Kalenichenko and Weijun Wang and Tobias Weyand and Marco Andreetto and Hartwig Adam},
    year={2017},
    eprint={1704.04861},
    archivePrefix={arXiv},
    primaryClass={cs.CV}
}


SSD Citation:
@article{Liu_2016,
   title={SSD: Single Shot MultiBox Detector},
   ISBN={9783319464480},
   ISSN={1611-3349},
   url={http://dx.doi.org/10.1007/978-3-319-46448-0_2},
   DOI={10.1007/978-3-319-46448-0_2},
   journal={Lecture Notes in Computer Science},
   publisher={Springer International Publishing},
   author={Liu, Wei and Anguelov, Dragomir and Erhan, Dumitru and Szegedy, Christian and Reed, Scott and Fu, Cheng-Yang and Berg, Alexander C.},
   year={2016},
   pages={21–37}
}

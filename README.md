# DhakaAI2020

### Introduction
DhakaAI 2020 challenge is a Traffic Detection with AI competition organized by Dhaka AI. The capital city of Dhaka has only 7% traffic roads (compared to 25% urban standard) in presence of approximately 8 million commuters a day within 306 sq km area. The scenario of Dhaka traffic is unique which poses complex new challenges in terms of automated traffic detection. To solve the problem using advances in AI-based technology and ICT solutions, we are calling for solutions to automatic Dhaka traffic detection problems on optical images. This new AI-Based Dhaka Traffic Detection Challenge aims at assessing the ability of state-of-the-art methods to detect and recognize traffic vehicles. This solution is encountered in modern cities where multiple cultures live and communicate together, where users see various scripts and languages in a way that prevents using much a priori knowledge. Also, at the same time, academics and researchers from the region who are experts in AI or interested in exploring possibilities could be brought to a networking community through this campaign. Working together on a common problem statement can create the right synergies needed to build an AI-based community in South-East Asia.

### What was the challenge
The competition will happen online and within 2 rounds. In the first round, a training dataset would be provided with which the participants need to train a generalized object detection model to locate traffic vehicles and identify them on the 1st test dataset and generate a submission file following the prescribed format. Based only on the detection accuracy, the top 30% team will move to the 2nd round where they will be evaluated based on the detection accuracy on the 2nd test dataset, poster, presentation, and codes.

### Dataset Description
The dataset is composed of vehicle images, where an image contains a vehicle of one or more of 21 different classes of vehicle. This makes the dataset useful for multiple vehicle detection and recognition. The considered vehicle classes are: ambulance, auto-rickshaw, bicycle, bus, car, garbage van, human hauler, minibus, minivan, motorbike, Pickup, army vehicle, police car, rickshaw, scooter, Suv, taxi, three-wheelers (CNG), truck, van, wheelbarrow.
**For this competition we also added around 100 images captured and labelled by ourself for training**.

### Code Description
For our approach we used a state of the art model for object detection model YOLO. We used an implementation of yolov5 by ultralytics and then customized some part of it. First, we needed to convert the VOC (.csv) labelling to YOLO trainable format (.txt). It was done with Data Preprocessing Notebook. Then we trained with ```(Training_Model)YOLOv5_(Custom)_Dhaka_Traffic_Detection_Starter_Notebook.ipynb``` notebook. Overall, for final submission we trained 4 different model with different target resolutuion and folding and then ensembeled these four weights in the inference. The custom version of yolov5 is also provided with this repository in Custom yolov5 folder.

### Team Members
<ul>
<li>Raian Rahman</li>
<li>Zadid Bin Azad</li><br>
Dept. of Computer Science and Engineering <br>
Islamic University of Technologylogy
</ul>

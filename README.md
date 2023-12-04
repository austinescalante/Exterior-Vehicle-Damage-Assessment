# Exterior Vehicle Damage Assessment and Classification Using Deep Learning

# Purpose of the Project
In an era where accidents are more prevalent, our goal is to transform the approach to evaluating and managing exterior vehicle damage. The objective of this work is to develop a trained detection system pipeline using deep learning to assess and classify exterior vehicle damage to provide a concise cost estimation of the car repairs. 

# Procedure
We have developed this system into three phases: Car Object Detection using Yolov8, Binary Classification of Damage and Segmentation of Damage using Yolov8. The Car Object Detection phase uses Yolov8 pretrained weights to identify car objects in the initial user image. The Binary Classification phases utilized the pretrained model, MobileNetV2 and the technique, transfer learning to train on damaged and undamaged image dataset. The Segmentation phase uses a dataset of 7,023 images classified into 4 categories: Wreck, Broken Glass, Scratch, and Dent to identify and create a mask of the damaged area. A price range based on the square feet of damage area was implemented to calculate total cost of repairs.

# Results
The implemented pipeline was able to successfully identify and classify car damage images into either of the four classes and produce a cost estimation range of the repairs in the binary classification phase, multiple CNN Classification models were trained to detect damage present in the car detected images. The MobileNetv2 model had the highest precision, recall and validation accuracy at 92% detecting the presence of damage. In the segmentation phase the score for the aggregate class classification resulted in a score of 0.902, meaning, indicating the model excels in accurately detecting and classifying objects across multiple classes. In addition, the mask mAP50 of the aggregate classes resulted in a high score of 0.885 signifying a strong performance in accurately detecting and localizing the damage objects with masks. The damage portions of the car images were able to be localized and identified by an instance segmentation mask. 

# Conclusion
Using this detection pipeline provided better assessment on the types of damage identified on a vehicle. The implementation of the detection pipeline allows for an efficient method into analyzing the cost associated with the damage portions of a car and accurate visibility of the damage associated with a crash.

![image](https://github.com/austinescalante/Exterior-Vehicle-Damage-Assessment/assets/60208327/6d024265-d91a-4a24-bd26-5ebd1da646d9)



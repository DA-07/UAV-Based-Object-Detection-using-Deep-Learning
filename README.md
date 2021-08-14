# UAV-Based-Object-Detection-using-Deep-Learning
Deep learning based object detection solutions incorporated with computer vision has been into spotlight amongst researchers and developers in recent years and has become one of the major Industry 4.0 technologies. Industries are endeavouring to solve a wide variety of robotic tasks in the areas of perception, planning, localization, and control by deploying these solutions. The flourishing UAV market interests in integration of mobile and ubiquitous computing using deep learning methodologies for potential applications like object detection, visual navigation, and surveillance with the vision of moving the processing tasks closer to the data source rather than routing the data to a central node.<br/>

This thesis work focuses on prototyping small-sized UAVs with mobile and ubiquitous computing capabilities, equipped with onboard GPU which is capable of real-time object detection with aerial bird’s-eye view. For achieving this, through a literature survey the state-of-the-art deep learning algorithms are tested and deployed on NVIDIA Jetson TX2 board which is a power-efficient embedded edge-AI device. Cars are the selected object for the object detection task in this thesis. Supervised learning approach is used for training the object detector with custom CARPK and PUCPR+ dataset. Data augmentation techniques are employed to increase the size of the dataset for improving the learning ability of the models like the novel Mosaic data augmentation which stitches 4 images together for improving the detection of small objects in YOLOv4 model. The training and validation of the fine-tuned YOLOv4, Tiny-YOLOv4, and YOLOv3 models with the custom dataset is done on Google Colab which provides free cloud Nvidia GPUs and the trained weights are saved. Lastly, testing is done with the optimum weights along with the testing model configurations on NVIDIA Jetson TX2 board.<br/>

The deployed solution in this thesis on NVIDIA Jetson TX2 board with MAX-N mode results in achieving real-time performance with fine-tuned Tiny-YOLOv4 model at a speed of 19-21 FPS, 97% precision, 87% F1-score, and 86.95% mAP; fine-tuned YOLOv4 (4 FPS, 95% precision, 96% F1-score, and 97.03% mAP); and fine-tuned YOLOv3 (3 FPS, 96% precision, 94% F1-score, and 95.47% mAP).<br/>

The results indicate that the customized Tiny-YOLOv4 model has the potentiality of real-time object detection with highest FPS of 21 and the customized YOLOv4 model with highest mAP of 97.03% and 96% of F1-score.<br/>

# Output Results on NVIDIA Jetson TX2:
[Video link of Demonstration](https://user-images.githubusercontent.com/71173101/129432310-c8ec9373-734b-4855-b2d2-cd395080d23c.mp4) <br/>

## Tiny-YOLOv4 Output:
![yolov4Tiny](https://user-images.githubusercontent.com/71173101/124332900-fbbb5b00-db92-11eb-8c12-1937c6b6a79f.gif) <br/>

## YOLOv4 Output:
![yolov4](https://user-images.githubusercontent.com/71173101/124333464-94060f80-db94-11eb-9d17-f98379b256ab.gif) <br/>

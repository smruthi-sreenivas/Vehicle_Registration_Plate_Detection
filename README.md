Object detection has a huge application in the industry. ANPR (Automatic Number Plate Recognition) is an integral part of the Electronic Toll Collection. 

Project Overview: Developed a robust vehicle registration plate detection system using computer vision techniques, leveraging YOLO (You Only Look Once) for object detection. The project involved downloading datasets, preprocessing images, and training a model to identify and localize vehicle registration plates in images and videos.

Key Components:
Data Acquisition and Preparation:

File Downloading: Implemented functions to download and unzip datasets from remote URLs, ensuring seamless data acquisition for training and validation.
Image and Label Loading: Developed functions to load images and their corresponding labels, applying regular expressions to extract relevant bounding box coordinates for vehicle registration plates.
Image Processing:

Bounding Box Conversion: Converted bounding box coordinates from YOLO format to standard coordinates (xmin, ymin, xmax, ymax) to facilitate accurate object localization in images.
Visualization: Created functions to plot images with bounding boxes overlaid, enabling visual validation of detected regions for quality assurance.
Model Training and Validation:

Dataset Structuring: Organized the dataset into training and validation directories, maintaining the appropriate structure for YOLO model training.
Model Evaluation: Integrated a model validation routine to assess performance using metrics like Mean Average Precision (mAP), achieving the following results:
mAP: 68.5%
mAP@0.50: 91.7%
mAP@0.75: 81.3%
mAP@0.50:0.95: 68.5%
Inference and Results Visualization:

Detection Functionality: Developed a function to run the trained model on images, displaying the results in real-time, and printing bounding box coordinates along with confidence scores for detected plates.
Video Processing: Extended the model to process video inputs, applying real-time detection on video frames and saving the annotated output.
Technologies Used:
Python, OpenCV, PyTorch, YOLOv5, NumPy, Matplotlib, and various Python libraries for data handling.
Achievements:
Successfully implemented a high-accuracy vehicle registration plate detection system, achieving significant improvements in detection speed and accuracy compared to traditional methods.
Enhanced user experience by providing real-time feedback and visual validation of detection results.

You can view the logs here:
https://api.wandb.ai/links/student_smruthi/0oaasbuc

Output video link:
https://www.youtube.com/watch?v=Io2EJXMALHs

Precision Recall Curve:
![image](https://github.com/user-attachments/assets/166ad49a-d5be-4e64-ae63-61d167ebe4f7)

Confusion Matrix:
![image](https://github.com/user-attachments/assets/35964524-1e7d-4e92-80f1-936314762fd2)




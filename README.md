Object detection has a huge application in the industry. ANPR (Automatic Number Plate Recognition) is an integral part of the Electronic Toll Collection. 

I have plotted Ground Truth bounding boxes and displayed few images with bounding boxes. I have used YOLOv9c from Ultralytics to train and detect registration plates.
Our labels are in xmin, ymin, xmax, ymax format. Inorder to use in YOLO, we need to convert that to YOLO format (xcenter,ycenter, width, height) and normalize them.

Validation metrics:
map  0.6846835531785074
map50  0.916618003272932
map75  0.8126096142676082
maps50-95  [    0.68468]

You can view the logs here:
https://api.wandb.ai/links/student_smruthi/0oaasbuc

Output video link:
https://www.youtube.com/watch?v=Io2EJXMALHs

Precision Recall Curve:
![image](https://github.com/user-attachments/assets/166ad49a-d5be-4e64-ae63-61d167ebe4f7)

Confusion Matrix:
![image](https://github.com/user-attachments/assets/35964524-1e7d-4e92-80f1-936314762fd2)




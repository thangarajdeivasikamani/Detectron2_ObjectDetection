# Detectron2 Object Detection
This repo contains local PC,Colab and flask based object detect web application based on Facebook detection framework.

##Data set:
 https://www.kaggle.com/datasets/nguyngiabol/colorful-fashion-dataset-for-object-detection

##Colab Training Procedure:

1. Download the above the data set and upload the JPG folder & Json file
2. If you have ( xml annotation file use voc2coco_predefined.py convert xml to json file format.
3. If your planning to create own annotate data set use labeling windows software
4. Register the dataset
5. Download the required model file from detectron2 zoo document page link.
6. Merge the required model config file  with base config file
7. Download the required model checkpoint.
8. Configure the few required parameters , like number of class
9. Train and store the model weight into required output folder ( model_final.pth)
10. Using saved model predict the new image for that select the few sample image & visualize.
11. Using detectron2.utils.visualizer import ColorMode predict the object from the BW and Color images.
12. Train with different model & continue the experiment.

## Web Application:

Download the pre_Trained model: https://drive.google.com/file/d/1UxXb3Z04NCQM3EIu-APWQ15GJCllA0HZ/view?usp=sharing

####Use age of web application:

1. Clone the repo
2. Copy the Pre_Trained model into main folder
3. Install the required package using requirements.txt
4. Run python clientApp.py
5. Open the URL in Browser
6. Upload the sample image
7. Press detect.


## Result
class_dict: {'bag': 1, 'dress': 2, 'hat': 3, 'jacket': 4, 'pants': 5, 'shirt': 6, 'shoe': 7, 'shorts': 8, 'skirt': 9, 'sunglass': 10}

Detected_classes: [8, 6, 1, 6]



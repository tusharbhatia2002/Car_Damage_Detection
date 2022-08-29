# Car_Damage_Detection
Object Detection machine learning model
<br />
#### Aim : 
     To train an object detection model using Tensorflow object detection API.
##
     
     
#### Dataset : 
  [Drive link](https://drive.google.com/drive/folders/1TiN2qCCmbhxrbV4JPNGGkzP0TA_850tb)
  
  
 ##   

#### Process : 
    1. Data annotation and cleaning : 
            a. Split the datasets into train and test data.
            b. Using LabelImg library to annotate the images. The annotated data was saved in .xml file which consists the co-ordinates of region of intrests. 
            c. The .xml files in both train and test dataset was further converted into .csv files. 
            d. Generated .tfrecords files using .csv files for each image in  train and test datasets. 

    2. Pre-trained model selection : 
            a. selected ssd_mobilenet_v1_coco model because of its goog accuracy. 

    3. Configuring .pbtxt and .config file : 
            a. Generated a .pbtxt file which consists of labels. In this case "scratch", "dent" and "replacement" was used. 
            b. Configured .config file. path to training data, evaluation data, number of classes, batch size, number of steps were configured to initiate the training process.

    4. Training the model : 
           a. Trained the model using : 
                                a. batch size = 24
                                b. num_step = 25k
                                c. number of hrs trained = 2:30 hrs 
                                d. loss of saved model = 1.3% 
                                e. The model was trained on Google Colab for accessing the better resource like GPU. 
                                

##

#### Libraries used : 
        1. Tensorflow 
        2. LabelImg 
        3. Numpy 
        4. OS
        5. Matplotlib
        6. Tensorboard 
        
##

#### Model Used :
     ssd_mobilenet_v1_coco model
     
##

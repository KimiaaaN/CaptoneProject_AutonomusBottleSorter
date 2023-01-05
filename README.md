# CaptoneProject_AutonomusBottleSorter

Autonomus Bottle sorter  is a computer vision project which  by training YOLOv4 model, we were able to achieve classification of the bottle types(glass, plastic, metal cans) with minimum accuracy of 91%.
 
We implemented our code in python, using the Google Colab environment for accesing its high GPU.
The most important libraries that we imported were CV2, numpy, matplotlib, Tensorflow as well as some essential functions from Google Colab to access the webcam properly.
We also used JavaScript to properly create our live video stream using our webcam as input.
 
 In this project, we used a trained YOLOv4 model by importing [DarkNet Repo](https://github.com/AlexeyAB/darknet),and enabling our GPU and OpenCV through the clonedfolder.
 
As we need GPU for training our model we also had to verify CUDA compiler driver to
guarantee that it is functioning and that the available version is compatible with the TensorFlow
version and GPU unit. 

For this project, The dataset we used is from Kaggle gathered by [Arkadiy Serezhkin](https://www.kaggle.com/datasets/arkadiyhacks/drinking-waste-classification?resource=). We used a total of 4820 RGB images from this dataset along with a txt file for each image. This dataset actually contains 4 classes, AluCan (Aluminum Can), Glass bottles, PET plastic bottles, and HDPEM plastic (which is like detergent bottles and big milk plastic gallons). Since we were focusing on a specific size of bottles which is a maximum of 750ml, we only eliminated HDPEM from the dataset. We also gather and add some data ourselves to this dataset.

This dataset is split into two sections: 80% for training and 20% for testing and validation.
For watching the damo of this project you can visit my [LinkedIn page here](https://www.linkedin.com/posts/kimia-nahravanian-0a60791b4_computervision-yolo-recycling-activity-6942226947070402560-iep9?utm_source=share&utm_medium=member_ios)

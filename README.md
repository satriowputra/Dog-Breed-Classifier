[//]: # (Image References)

[image1]: ./images/sample_dog_output.png "Sample Output"
[image2]: ./images/vgg16_model.png "VGG-16 Model Layers"
[image3]: ./images/vgg16_model_draw.png "VGG16 Model Figure"


## Project Overview

In this project, I  learn how to build a pipeline that can be used within a web or mobile app to process real-world, user-supplied images.  Given an image of a dog, my algorithm will identify an estimate of the canine’s breed.  If supplied an image of a human, the code will identify the resembling dog breed.  

![Sample Output][image1]

Along with exploring state-of-the-art CNN models for classification and localization, I made important design decisions about the user experience for my app.  My goal is that by completing this lab, I understand the challenges involved in piecing together a series of models designed to perform various tasks in a data processing pipeline.  Each model has its strengths and weaknesses, and engineering a real-world application often involves solving many problems without a perfect answer. Imperfect solution will nonetheless create a fun user experience!

## Installation

1. Clone the repository and navigate to the downloaded folder.
	
	```	
		git clone https://github.com/satriowputra/Dog-Breed-Classifier.git
	```
    
__NOTE:__ Please note that i am running this notebook inside Udacity workspace. Remove any `active_session()` function from the notebook to prevent error.

2. Download the [dog dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip).  Unzip the folder and place it in the repo, at location `path/to/dog-project/dogImages`.  The `dogImages/` folder should contain 133 folders, each corresponding to a different dog breed.
3. Download the [human dataset](http://vis-www.cs.umass.edu/lfw/lfw.tgz).  Unzip the folder and place it in the repo, at location `path/to/dog-project/lfw`.  If you are using a Windows machine, you are encouraged to use [7zip](http://www.7-zip.org/) to extract the folder. 
4. Make sure you have already installed the necessary Python packages according to the README in the program repository.
5. Open a terminal window and navigate to the project folder. Open the notebook and follow the instructions.
	
	```
		jupyter notebook dog_app.ipynb
	```
__NOTE:__ Make sure you have PyTorch installed on your machine prior using the notebook.

__NOTE:__ There are also several libraries that i used here that should be installed if you are install Python from Anaconda Distribution such as: Numpy, Matplotlib, time, cv2, tqdm, and PIL.

## File Description

There are several files and picture I uploaded here:
1. workspace_utils.py: contains function to prevent workspace being disconnected while running long processes.
2. /haarcascade: contains parameter used in face detection algorithm.
3. /images: iamges used in notebook.
4. /custom_image: images used to test classifier algorithm.


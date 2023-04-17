# Pakistani_Celebrity_Image_Classifier_CNN
The Dataset has been collected by using Chrome Extension "Download All Images". After doing some data preprocessing apply CNN model.

## Libraries Used:<br>
1. cv2 <br>
2. numpy<br>
3. matplotlib<br>
4. os<br>
5. shuttle<br>
6. Tensorflow<br>
7. Keras<br>
8. imghdr<br>

# Steps Involved:<br>
### 1. Importing the above mentioned libraries<br>
### 2. Data Cleaning<br>
  In this step I clean data by using HardCodeCase .xml files in which detect eyes and face of the actors and implements the changes. Furthermore, I make a new cropped image folder in which save all the cropped images.<br>
  Secondly, delete the images that was got cropped but the faces was not of the same person so delete those files.<br>
  Lastly, delete those images those were blur or not was looking good to model.<br>
### 3. Preprocessing the images:<br>
  Preprocessing is crucial so model can perform best so I make a function in which if images have any wrong format image then delete this image.<br>
### 4. Make a pipeline:<br>
  Pipeline is made by using tensorflow.keras.utils and store all the into batches for further model building<br>
### 5. Scaling:<br>
  After making batches of the data then scale these images so each image has proper same size because model only can take the same size image not different.<br>

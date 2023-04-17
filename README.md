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
### 6. Split the Data:<br>
  Data spliting is done by dividing the whole data into 3 parts train,test and validation data. The train has 70%, test has 20% and validation has 10% of the total data.<br>
### 7. Model Building:<br>
  Model is build in Deep Neural Network in which there are 9 different layers first 6 are Cov2d and MaxPool which have different units and same filters and activation.
  The 7 layer is flatten layer to flat the data into 1d. The last two layers are Dense layers. In output layer the activation function is "Softmax" because having 10 different classes.
  Then compile the data with loss= sparse_categorical_features and optimizer is "adam".
### 8. Performance check:
  The performace of this model is really accurate with 98.44% accuracy and with minimum loss(0.06).




# Screen Shots:


![image](https://user-images.githubusercontent.com/104086680/232634486-ff0c5208-4577-4fd5-88f2-0d16147bfe20.png)



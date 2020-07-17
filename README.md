
# **Behavioral Cloning Project**
This project is Implementation of the paper "End to End Learning for Self-Driving Cars"

**Goals / Steps**:
* Use the simulator to collect data of good driving behavior
* Build, a CNN model in Keras that predicts steering angles from images
* Train and validate the model with a training and validation set
* Test that the model successfully drives around track one without leaving the road







#### Dataset

To train my model I used dataset provided by Udacity. And the data is divided into 80% training data and 20% validation data. Some of the samples from original dataset are

| Camera | Image 1 | Image 2 |
| ---- | ---- | ---- |
| **Center Camera Images** | ![alt text](/Data/center1.jpg "Center Images") | ![alt text](/Data/center2.jpg "Center Images") |
| **Left Camera Images** | ![alt text](/Data/left1.jpg "Left Images") | ![alt text](/Data/left2.jpg "Left Images") |
| **Right Camera Images** | ![alt text](/Data/right1.jpg "Right Images") | ![alt text](/Data/right2.jpg "Right Images") |



 After cropping image I applied normalization on images and these normalized images are passed to the network as input. I used this training data for training the model. The validation set helped determine if the model was over or under fitting. I used an adam optimizer so that manually training the learning rate wasn't necessary.

### Evaluation Video

<p align="center">
  <img src="Evaluation.gif">
</p>

# CNN_Big_Cat_Classification

This notebook uses the "10 Big Cats of the Wild" Dataset from [kaggle](https://www.kaggle.com/datasets/gpiosenka/cats-in-the-wild-image-classification?datasetId=2949345). The 'code' section of the notebook contains all of the code that I used to build a image classification model using tensorflow and keras. I used a convolutional neural network with transfer learning to train the model. The model I used for transfer learning was [resnet_50_v2](https://tfhub.dev/google/imagenet/resnet_v2_50/feature_vector/5).
>
The accuracy on the training data was 98% and the accuracy on the testing data was 100%. Below you can see the loss and accuracy curves, as well as a confusion matrix:

### Accuracy Curve:
![acc](/CNN_Big_Cat_Classification/images/accuracy.png)

### Loss Curve:
![loss](/CNN_Big_Cat_Classification/images/loss.png)

### Confusion Matrix:
![CM](/CNN_Big_Cat_Classification/images/matrix.png)

---
Finally I also created a very basic front end application in the 'app' notebook using Flask. The app allows you to insert a photo into it, which is then preprocessed and fed into the CNN that was built and makes a prediction on the animal. Below is a picture of the front end after passing a picture of a Lion to the model.
![frontend](/CNN_Big_Cat_Classification/images/Capture.PNG)
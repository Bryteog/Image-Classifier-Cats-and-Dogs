#### Overview

Built a model to classify images of cats and dogs. The dataset is obtained from kaggle [Cats and Dogs](https://www.kaggle.com/competitions/dogs-vs-cats/data). The data is made up of two directories of cats and dogs images.


#### Model

Image preprocessing via flipping, rescaling, normalising, zooming and rotation is applied to the train set only. The Resnet50 and efficientnet pretrained model is used for training, the last layer is changed to reflect the number of classes. The model has two versions due to the different pretrained layers used.
The accuracy of training and testing sets for version 1 after 10 epochs is 98.2% and 94.8% respectively with losses of 0.046 and 0.1324. Version 2 after 25 epochs of training had 96.3% and 88.72% accuracy and losses of 0.1019 and 0.3533 for both the training and testing sets respectively. Indicating the second version began to overfit after a while. 
## Update the accuracy and losses for v3
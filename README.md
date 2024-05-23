# Potato disease classification :

Project statement is to classify whether a plant is healthy or not by using an image of a potato leaf.
It is a multi-class classification problem.
Following are the three classes:

• Late Blight- Potato leaves are more deteriorated.

• Early Blight- Potato leaves are in the early stage of disease.

• Healthy- Leaves are healthy.

# Technical diagram :
![td](https://github.com/muditprakash/potato-disease-classifier/assets/75181670/6f6ef2de-e91f-44c6-b529-c61bab2316aa)

### Plant Village: Potato Leaf Image Dataset

This folder contains labeled images of potato leaves, which will serve as our primary data source for this project.

#### Data Cleaning and Pre-processing

We imported the dataset using TensorFlow (tf) methods. The dataset consists of 2,152 files belonging to three different classes. In this step, we partitioned the data into training, test, and validation sets and stored it in such a way that we can use optimal resource allocation while using it. 

We normalized the images using the `resize and rescale method` and then performed `data augmentation` to enhance the chances of obtaining a high-accuracy model.

### Model Building

We used the standard `CNN` model coupled with the `softmax` activation function. The model architecture is:

![model architecture](https://github.com/muditprakash/potato-disease-classifier/assets/75181670/23c5df7f-9024-471c-970c-c9550438769b)



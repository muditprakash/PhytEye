# <p style="text-align: center;">PhytEye</p>

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

Then we compiled the model using ``` adam``` optamizer and using ``` accuracy``` as the evaluation metrics and ``` sparse catagorical entropy ``` as a loss trained it till 50 ``` epochs``` .

### Model Validation 
We achieved a very high accuracy of 96% on our test dataset. Here is the training vs validation graph showing the model performance:
![output](https://github.com/muditprakash/potato-disease-classifier/assets/75181670/902679b1-aa60-44c2-9004-fe443f441eab)

### Model saving and fastapi :

Once we achieved the desired result, it was time to save the model. Here, we are saving the model in h5 file format and using FastAPI to serve the model.

# Running it locally:

clone the repo 
```
git clone https://github.com/muditprakash/potato-disease-classifier.git
```
Install requirements.txt file 
```
pip install -r requirements.txt
```
Run main.py as 

```
python main.py
```






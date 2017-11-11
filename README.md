# Simpsons_Characters_classification
Download the dataset from here: https://www.kaggle.com/alexattia/the-simpsons-characters-dataset/data


# Pre-Requisites
- Tensorflow (tensorflow-gpu if you will to re-train the model)
- Keras
- numpy

# ResNet Architecture
### Identity Block
- resnet.py
![Image of Identity Block](https://raw.githubusercontent.com/damgambit/simpsons_characters-classification/master/images/idblock3_kiank.png)

### Convolutional Block
- resnet.py
![Image of Convolutional Block](https://raw.githubusercontent.com/damgambit/simpsons_characters-classification/master/images/convblock_kiank.png)

### Classic ResNet50
![Image of ResNet50](https://raw.githubusercontent.com/damgambit/simpsons_characters-classification/master/images/resnet_kiank.png)


# Perfomances
### Optimizer Adam:
- Learning Rate = 0.001
- Beta1         = 0.9
- Beta2         = 0.999
- epsilon       = 1e-08
- decay         = 0.002

### Callbacks
- EarlyStop
- Reduce Learning Rate on Validation Loss plateu
- ModelCheckPoint

### Loss&Metrics
- Categorical CrossEntropy
- Accuracy

### Training
- BatchSize     = 64
- Epochs        = 500 (40)


## Training Accuracy: 0.9998
![Image of Training Accuracy](https://raw.githubusercontent.com/damgambit/simpsons_characters-classification/master/images/acc_train.PNH) 
## Testing Accuracy: 1
![Image of Testing Accuracy](https://raw.githubusercontent.com/damgambit/simpsons_characters-classification/master/images/acc_test.PNH) 

## Training Loss: 0.0012
![Image of Training Loss](https://raw.githubusercontent.com/damgambit/simpsons_characters-classification/master/images/loss_train.PNH) 
## Testing Loss: 0.0014
![Image of Testing Loss](https://raw.githubusercontent.com/damgambit/simpsons_characters-classification/master/images/loss_test.PNH) 

Thank you!
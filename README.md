# Simple-Image-Classifier
Model that able to distinguish picture between dog, cat, or panda.
<center>
<img src='bground.jpg'>
  </center>

Dataset were taken from <a href ='https://www.kaggle.com/ashishsaxena2209/animal-image-datasetdog-cat-and-panda'>Kaggle</a>

Dataset has 1000 picture of each cat, dog, and panda. Then I divided into train : test with test_size ratio of 0.2

This model were make using keras - tensorflow with Sequential model

Here is the summary :
Model: "sequential"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
average_pooling2d (AveragePo (None, 49, 49, 1)         0         
_________________________________________________________________
conv2d (Conv2D)              (None, 47, 47, 16)        160       
_________________________________________________________________
conv2d_1 (Conv2D)            (None, 45, 45, 16)        2320      
_________________________________________________________________
max_pooling2d (MaxPooling2D) (None, 22, 22, 16)        0         
_________________________________________________________________
dropout (Dropout)            (None, 22, 22, 16)        0         
_________________________________________________________________
flatten (Flatten)            (None, 7744)              0         
_________________________________________________________________
dense (Dense)                (None, 512)               3965440   
_________________________________________________________________
dense_1 (Dense)              (None, 3)                 1539      
=================================================================
Total params: 3,969,459
Trainable params: 3,969,459
Non-trainable params: 0

This model is able to predict with up to 71% accuracy.

As I will keep learning about deep learning, I believe this model's accuracy STILL can be improved.

#### Thankyou and Happy Coding :)

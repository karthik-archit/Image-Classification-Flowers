# Image-Classification-Flowers
Classification of flowers , by finetuning Resnets and Inception models also image augmentation and random image erasing 

Overview :

Image classification of flowers into 104 different categories. Various pre-trained models like Resnets , VGG-19 , Inception were studied and fine tuned for this task to find the best fit. Considering the smaller dataset , and 104 different flowers , models can result in overfitting pretty quickly, so data augmentation techniques were used , also random image erasing were used. Various tensorflow functions were used, especially using tensorflow datasets , and how to optimize them to run on TPU’s.

Dataset Source :

Kaggle Competition Dataset - https://www.kaggle.com/competitions/tpu-getting-started/data

Libraries Used :

Keras, Tensorflow, Pandas, Numpy.

Project Flow :

Importing data -> unpacking data from tfrecords -> extract images and labels -> decoding images -> apply data augmentation -> perform random erasing of images -> fetching the optimized datasets for training and validation data -> training the model -> evaluation 

Augmentations applied :
Random Flip

Random Rotation

Random Translation

Random Zoom 

Models Used and their accuracies :

Inception V3 with custom head  - 85

Resnet 50 with custom head – 80

Through this project was able to understand the intuition behind VGG-19 , Resnets , Inception models , the intuition of stacking CNNs, problem of vanishing gradients etc. This also helped in understanding of transfer learning and finetuning models based on our need . Got familiar with tensorflow functions and datasets and how to improve efficiency using them . Understood the need for data augmentation and also how it helps in improving the generalization of the models.





# Fine-tune-realTime-face-detector

It present a few simple yet effective methods that you can use to build a powerful image classifier, using only very few training examples --just a few hundred or thousand pictures from each class you want to be able to recognize. It also shows how the real-time image classification works.

## Main files

`FineTune_and_Data_Augmentation.ipynb` includes the main classifcation code. 

the outline will go as follows:
- collection data from the kaggle [cats_and_dogs](https://www.kaggle.com/c/dogs-vs-cats/data) and use only 2800 data points, where `2000` for training and validation and `800` for validation. we also use extra `400` for testing
- training a small network from scratch as a baseline
- apply the data augmentation
- using the bottleneck features of a pre-trained network
- fine-tuning the top layers of a pre-trained network

The main purpose is to familar with some Keras features:
- `fit_generator` for training Keras a model using Python data generators
- `ImageDataGenerator` for real-time data augmentation
- `layer freezing and` model fine-tuning

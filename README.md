# Image_caption_generator

This is implementation of a image caption generator which generates a caption based on the things that are present in the image. Image captioning is a challenging task where computer vision and natural language processing both play a part to generate captions.

Datasets used: FLICKR_8K : It contains 8,000 images that are each paired with five different captions which provide clear descriptions of the salient entities and events. 

Flow of the project:

- Cleaning the caption data
- Extracting features from images using VGG-16
- Merging the captions and images
- Building LSTM model for training
- Predicting on test data
- Evaluating the captions using BLEU scores as the metric.

Recommended System Requirements to train model.

    A good CPU and a GPU with atleast 8GB memory
    Atleast 8GB of RAM
    Active internet connection so that keras can download inceptionv3/vgg16 model weights

Required libraries for Python :

    Python 
    Numpy 
    Tensorflow 
    Keras 
    nltk 
    PIL 
    Matplotlib 
    
using VGG16 model + RNN with epochs 10 and optimizer 'Adam'
```
BLEU-1: 0.542497
BLEU-2: 0.292949
BLEU-3: 0.193336
BLEU-4: 0.083422

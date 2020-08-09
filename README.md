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

**Recommended System Requirements to train model. **

A good CPU and a GPU with atleast 8GB memory
Atleast 8GB of RAM
Active internet connection so that keras can download vgg16/inceptionV3 model weights

Required libraries for Python :

- Python 
- Numpy 
- Tensorflow 
- Keras 
- nltk 
- PIL 
- Matplotlib 
    
## Results    
- Using VGG16 model + RNN with epochs 10 and optimizer 'Adam'
`
    BLEU-1: 0.542497
    BLEU-2: 0.292949
    BLEU-3: 0.193336
    BLEU-4: 0.083422
    `
- Using inceptionV3 model + RNN with epochs 10 and optimizer 'Adam'
`
    BLEU-1: 0.560461
    BLEU-2: 0.304736
    BLEU-3: 0.198677
    BLEU-4: 0.086893`
    
  ### Future Works:
  - Implementation of Beam Search Algorithm
  - Use of alternate Pre-Trained Photo Models like Resnet50.
  - Use of Pre-trained Word Vectors

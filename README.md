# Image_caption_generator

This is implementation of a image caption generator which generates a caption based on the things that are present in the image. Image captioning is a challenging task where computer vision and natural language processing both play a part to generate captions.

Datasets used: FLICKR_8K : It contains 8,000 images that are each paired with five different captions which provide clear descriptions of the salient entities and events. 
Flow of the project

- Cleaning the caption data
- Extracting features from images using VGG-16
- Merging the captions and images
- Building LSTM model for training
- Predicting on test data
- Evaluating the captions using BLEU scores as the metric

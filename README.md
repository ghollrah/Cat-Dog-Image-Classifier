# Cat-Dog-Image-Classifier

This is a set of models created to classify whether an image contains either a dog or a cat. One model was trained using Logistic Regression, while the other model was trained with a Convolutional Neural Network. Using a dataset containing 5,000 pictures of cats and 5,000 pictures of dogs, the data was split so that 80% of the data would be used for training and the remaining 20% of the data would be used for testing. 

# Data Pre-Processing

Each image is read in and converted to grayscale and resized to 64x64, producing a 3D NumPy array with the shape (64,64,1). This will be the x-data. When each image is read in, if the image filename contains the word 'cat', then it will be classified with the number 1, while an image filename containing the word 'dog' will be classified with the number 0. This will be the y-data. Once the images have been read in and converted, the x-data will be concatenated with the y-data to produce a 2D NumPy array containing the x-data and the y-data.

# Logistic Regression

The model trained using logistic regression was trained for 5000 steps with the following learning rates: 0.001, 0.003, 0.005, and 0.01. 

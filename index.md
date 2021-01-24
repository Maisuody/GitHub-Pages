## Welcome to Deep-Learning-Framework

This deep learning framework can be used primarily to build deep learning models with ease. it provieds many utilities such as: visualization costs with epochs, Evaluation metrics and more.

### Our project

in this project we implement our Neural Network , a Neural network is simply a function, mapping an input (such as an image) to a prediction. Fundamentally, there are two simple operations you want to do with a function: calculate the output and the derivative, given an input. The first one is needed to obtain predictions, the latter one is to train your network with gradient descent. In neural network terminology, calculating the output is called the forward pass, while the gradient with respect to the input is called a local gradient.

## our modules to build our neural network
- Data Module "loading dataset or split the data"
- core modules
  1- Layers
  2- Losses
  3- Activation functions
- Visualization Module "Visualize the cost function versus iterations/epochs during training process"
- Evaluation Module "Implement accuracy estimation function and implement precision & recall metric for better evaluation"
- Utility Module: "This module is for saving & loading model weights & configurations into a compressed format"

## Dataset :
```markdown
1-Download the dataset of  MNIST as a .csv file from kaggle
2-Create a specific folders for training, validation & testing.
3-Split randomly the training .csv file into training & validation dataset.
```
# First module
## load_data
def loadData(file_path, y , indexY):
y is the Label
indexY the index of label

def image(image_path): 
Take the image and make resize for image then return all pixels in the image

def normalization(pixels):
Normalize any input by dividing by 255 The max value

def split_dataset(all_pixels, Labels,testSize):
testSize is th size of train 
and Return x_train, y_train, x_tests , y_tests

## build layers
###  Layer
- Initialization for the parameters of the class layer
- input -- the input to the layer for forward propagation.
  return -- computes the output of a layer for a given input
- input -- dY = The gradient of the error with respect to previous layer,
  input -- learning_rate = learning rate to update weights.
  return -- computes the gradient of the error with respect to this layer and update parameters if any.
  
 ###  FC(Layer)

- Initialization for the parameters of the class fully connected layer
        input_size = number of input neurons
        output_size = number of output neurons

- input -- the input to the layer for forward propagation.
        Returns:
        return -- computes the output of a layer for a given input

- input -- dY = The gradient of the error with respect to previous layer,
        input -- learning_rate = learning rate to update weights.
        Returns:
        return -- computes the gradient of the error with respect to this layer and update weights.

### ActivationLayer(Layer)
- input -- activation = pass the name of the activation function,
        input -- learning_rate = pass the name of the activation function gradient.

- input -- the input to the layer for forward propagation.
        Returns:
        return -- computes the output of a layer for a given input

- input -- dY = The gradient of the error with respect to previous layer,
        input -- learning_rate = learning rate to update weights if any.
        Returns:
        return -- computes the gradient of the error with respect to this activation
        
### Flatten(Layer)    



```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/Maisuody/GitHub-Pages/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.

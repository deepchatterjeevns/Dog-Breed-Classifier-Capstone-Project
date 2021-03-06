# Udacity Data Science Nanodegree

##  Capstone Project - Dog Breed Classifier
The goal of this project is to detect the breed of a dog using Convolutional Neural Network (CNN) with at least 60% accuracy.




# Software Requirements
 Python 3.x
 Numpy
 Pandas
 Matplotlib
 Scikit-Learn
 Keras
 Tensorflow
 OpenCV
 
## Metrics:
For this project, the metric used is the accuracy score.

## File structure and desciption:

    |   .gitattributes
    |   dog_app.ipynb
    |   extract_bottleneck_features.py
    |   LICENSE
    |   README.md
    |   
    +---haarcascades
    |       haarcascade_frontalface_alt.xml
    |       
    +---images
    |       American_water_spaniel_00648.jpg
    |       Brittany_02625.jpg
    |       Curly-coated_retriever_03896.jpg
    |       Labrador_retriever_06449.jpg
    |       Labrador_retriever_06455.jpg
    |       Labrador_retriever_06457.jpg
    |       sample_cnn.png
    |       sample_dog_output.png
    |       sample_human_2.png
    |       sample_human_output.png
    |       Welsh_springer_spaniel_08203.jpg
    |       
    +---saved_models
    |       InceptionV3_model.weights.best.hdf5
    |       weights.best.from_scratch.hdf5
    |       weights.best.VGG16.hdf5
    |       
    \---test images
            Dodo.jpg
            Grate Dane.jpg
            Labrador Retriver.jpg
            Ryan Gosling.jpg
            Ryan Reynolds.jpg
            Scooby Doo.jpg
The above tree describes all the files as part of this project.
   - dog_app.ipynb The main file for this project, it contains all the codes and also has the outputs. 
   - extract_bottleneck_features.py : it is used as a module in the main file to extract bottleneck features
   - haar cascades: Contains the haarcascade XML file to be used by cascade classifiers for face detection.
   - saved_models: contains the saved best model weights of pre-trained models. It doesn't include InceptionV3 weights because of its large size to upload. It can be generated by training the model. Steps in the next section.
   - images and test images: images to test the model
## Steps to replicate the project
   - All the dependencies are in requirement.txt and requirements-gpu.txt. A new virtual environment is preferable.
   Using python
   python -m venv myenv
   
   using Anaconda distribution
   conda create --name myenv
   
   - Then all the dependencies can be installed using pip
   pip install -r requirements.txt
   
   - Clone the repo in new venv
   - Download the [dog image dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip). Unzip the folder   at      location path/to/dog-project/dogImages.
   - Download the [human image dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/lfw.zip). Unzip the folder at            location path/to/dog-project/lfw.
   - Download the [VGG-16](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogVGG16Data.npz) and [InceptionV3](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogInceptionV3Data.npz) bottleneck features for the dog dataset.
     Place it in the repo, at location path/to/dog-project/bottleneck_features.
   - Run the jupyter notebook
   
 ## Takeaways and final thoughts
 The InceptionV3 model achieves an accuracy of 80% after 20 epochs. The accuracy can be improved in various ways like increasing the number of epochs, trying other pre-trained models, etc. The next step for me is to create a web app that takes an image as an input, then gives the result as a breed of dog. I have also written an accompanying [Medium Blog](https://medium.com/@deepchatterjee./dog-breed-classifier-d2492a1d52b1).
 
 ## Acknowledgement and Licensing terms
 I am thankful to Udacity for providing such wonderful tutorials. All the datasets are provided by Udacity. Kindly refer to Udacity [Terms of Service](https://www.udacity.com/legal) for further information.
































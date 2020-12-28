# Gesture Recognition Case study IIITB Assignment

Developed by:

### Github Details:

<span style="color: green"> Rakesh Kumar </span>

[<img src="https://img.shields.io/badge/github-%2312100E.svg?&style=for-the-badge&logo=github&logoColor=white" />](https://github.com/RakeshKumar045?tab=repositories) [<img src="https://img.shields.io/badge/linkedin-%230077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white" />](https://www.linkedin.com/in/rakesh-kumar-gupta-52b77ab4/) [<img src = "https://img.shields.io/badge/kaggle-%3390FF.svg?&style=for-the-badge&logo=kaglle&logoColor=white">](https://www.kaggle.com/rakesh6184) [<img src = "https://img.shields.io/badge/twitter-3336FF.svg?&style=for-the-badge&logo=twitter&logoColor=white">](https://twitter.com/2702rakesh) [<img src="https://img.shields.io/badge/medium-%2312100E.svg?&style=for-the-badge&logo=medium&logoColor=white" />](https://medium.com/@2702rakesh)

<span style="color: green"> Trishala Singh Rajput </span>

[<img src="https://img.shields.io/badge/github-%2312100E.svg?&style=for-the-badge&logo=github&logoColor=white" />](https://github.com/Trishala-Sin?tab=repositories) [<img src="https://img.shields.io/badge/linkedin-%230077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white" />](https://www.linkedin.com/in/trishala-singh/) [<img src = "https://img.shields.io/badge/kaggle-%3390FF.svg?&style=for-the-badge&logo=kaglle&logoColor=white">](https://www.kaggle.com/trishalasingh) [<img src="https://img.shields.io/badge/medium-%2312100E.svg?&style=for-the-badge&logo=medium&logoColor=white" />](https://medium.com/@2702rakesh)

### Problem Statement

Imagine you are working as a data scientist at a home electronics company which manufactures state of the art smart
televisions. You want to develop a cool feature in the smart-TV that can recognise five different gestures performed by
the user which will help users control the TV without using a remote.

The gestures are continuously monitored by the webcam mounted on the TV. Each gesture corresponds to a specific command:

| Gesture | Corresponding Action |
| --- | --- | 
| Thumbs Up | Increase the volume. |
| Thumbs Down | Decrease the volume. |
| Left Swipe | 'Jump' backwards 10 seconds. |
| Right Swipe | 'Jump' forward 10 seconds. |
| Stop | Pause the movie. |

Each video is a sequence of 30 frames (or images).

### Objectives:

1. **Generator**:  The generator should be able to take a batch of videos as input without any error. Steps like
   cropping, resizing and normalization should be performed successfully.

2. **Model**: Develop a model that is able to train without any errors which will be judged on the total number of
   parameters (as the inference(prediction) time should be less) and the accuracy achieved. As suggested by Snehansu,
   start training on a small amount of data and then proceed further.

3. **Write up**: This should contain the detailed procedure followed in choosing the final model. The write up should
   start with the reason for choosing the base model, then highlight the reasons and metrics taken into consideration to
   modify and experiment to arrive at the final model.

### Installation:

Run ***pip install -r requirements.txt*** to install all the dependencies.

### Dataset:

You can download the dataset from [here.](https://drive.google.com/uc?id=1ehyrYBQ5rbQQe6yL4XbLWe3FMvuVUGiL)
The training data consists of a few hundred videos categorised into one of the five classes. Each video (typically 2-3
seconds long) is divided into a sequence of 30 frames(images). These videos have been recorded by various people
performing one of the five gestures in front of a webcam - similar to what the smart TV will use.It looks like this:
![dataset](https://user-images.githubusercontent.com/29462447/86066087-d03cf680-ba8e-11ea-91f5-960b5f522a39.png)

### Results:

![observations](https://user-images.githubusercontent.com/29462447/86066095-d501aa80-ba8e-11ea-82d8-4681e20e310e.png)

I choose CNN+LSTM based model as the final choice due to fairly decent accuracy considering the type of data as well the
no. of parameters as I wanted my model to be light weight in nature.


# MIDAS
<h1 align="center">MIDAS-An Intelligent Mask Detection System</h1>

<div align= "center">
  <h4>Face Mask Detection system built with OpenCV, Keras/TensorFlow using Deep Learning and Computer Vision concepts in order to detect face masks in static images as well as in real-time video streams.</h4>
</div>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
![Python](https://img.shields.io/badge/python-v3.6+-blue.svg)
[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/jelonmusk/midas/issues)
[![LinkedIn](https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555)](https://www.linkedin.com/in/juvairiya-fathima/)


&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
![](https://github.com/jelonmusk/midas/blob/main/image3.png)


## :innocent: Motivation
In 2020, the world changed. This project examines the coronavirus pandemic, the efforts to combat it and ways to manage its mental health toll and safety regulations. Also, the absence of large datasets of __‘with_mask’__ images has made the task of automated mask detection a challenge. 

 

## :warning: TechStack/framework used

- [OpenCV](https://opencv.org/)
- [Caffe-based face detector](https://caffe.berkeleyvision.org/)
- [Keras](https://keras.io/)
- [TensorFlow](https://www.tensorflow.org/)
- [MobileNetV2](https://arxiv.org/abs/1801.04381)

## :star: Features
Our face mask detector didn't use any morphed masked images dataset. The model is accurate, and since we used the MobileNetV2 architecture, it’s also computationally efficient and thus making it easier to deploy the model to embedded systems (Raspberry Pi, Google Coral, etc.).

In the current scenario, identification is manually performed by a person leading to inefficiency and inaccuracy, thereby demanding the need of human invigilator for monitoring.
Using MIDAS, an automated identification system is developed thus saving time and increasing accuracy.
It eliminates the need of human invigilation and provides easier integration and compatibility with major security devices.


## :file_folder: Dataset
The dataset used can be downloaded here - [Click to Download](https://drive.google.com/drive/folders/1FNcU446ROZQNDhUJKqvwNGEebpoklC7p?usp=sharing)

This dataset consists of __3835 images__ belonging to two classes:
*	__with_mask: 1916 images__
*	__without_mask: 1919 images__

The images used were real images of faces wearing masks. The images were collected from the following sources:

* __Bing Search API__ ([See Python script](https://github.com/jelonmusk/midas/blob/master/search.py))
* __Kaggle datasets__ 
* __RMFD dataset__ ([See here](https://github.com/X-zhangyang/Real-World-Masked-Face-Dataset))

## :key: Prerequisites

All the dependencies and required libraries are included in the file <code>requirements.txt</code> [See here](https://github.com/jelonmusk/midas/blob/master/requirements.txt)

## 🚀&nbsp; Installation
1. Clone the repo
```
$ git clone https://github.com/jelonmusk/midas.git
```

2. Change your directory to the cloned repo and create a Python virtual environment named 'test'
```
$ mkvirtualenv test
```

3. Now, run the following command in your Terminal/Command Prompt to install the libraries required
```
$ pip3 install -r requirements.txt
```

## :bulb: Working

1. Open terminal. Go into the cloned project directory and type the following command:
```
$ python3 train_mask_detector.py --dataset dataset
```

2. To detect face masks in an image type the following command: 
```
$ python3 detect_mask_image.py --image images/pic1.jpeg
```

3. To detect face masks in real-time video streams type the following command:
```
$ python3 detect_mask_video.py 
```
## :key: Results

#### The model gave 93% accuracy for Face Mask Detection after training via <code>tensorflow-gpu==2.0.0</code>

![](https://github.com/jelonmusk/midas/blob/main/accuracy.png)

#### The following accuracy/loss training curve plot
![](https://github.com/jelonmusk/midas/blob/main/plot.png)

## Streamlit app

MIDAS webapp using Tensorflow & Streamlit

command
```
$ streamlit run app.py 
```
## Images

<!-- <p align="center">
  <img src="https://github.com/jelonmusk/midas/blob/main/image2.png">
</p>
<p align="center">Upload Images</p>
 -->
<p align="center">
  <img src="https://github.com/jelonmusk/midas/blob/main/image2.png">
</p>
<p align="center">Results</p>

## :clap: And it's done!
Feel free to mail me for any doubts/query 
:email: jelonmusk@gmail.com

## :handshake: Contribution
Feel free to **file a new issue** with a respective title and description on the the [MIDAS](https://github.com/jelonmusk/midas/issues) repository. If you already found a solution to your problem, **I would love to review your pull request**! 

## :heart: Owner
Made with :heart:&nbsp;  by [JShaikh](https://github.com/jelonmusk)

## :+1: Credits
* [https://www.pyimagesearch.com/](https://www.pyimagesearch.com/)
* [https://www.tensorflow.org/tutorials/images/transfer_learning](https://www.tensorflow.org/tutorials/images/transfer_learning)

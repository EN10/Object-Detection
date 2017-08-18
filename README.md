# Object Detection

Based on: 
* [Tensorflow Object Detection API](https://github.com/tensorflow/models/tree/master/object_detection)
* [Installation](https://github.com/tensorflow/models/blob/master/object_detection/g3doc/installation.md)

## Install Tensorflow:

    sudo pip install -U pip  
    sudo pip install tensorflow 
    
## Install Jupyter
https://github.com/EN10/MNIST/blob/master/MoreExamples/installJupyter.txt

    sudo pip install pillow
    sudo pip install lxml
    sudo pip install jupyter
    sudo pip install matplotlib
    
## Install Protobuf 2.6+
As Ubuntu 14.04 has 2.5 download newer binary

    wget https://github.com/EN10/Object-Detection/raw/master/protoc
    sudo mv protoc /usr/bin/protoc
    
Source: https://github.com/google/protobuf/releases
    
    unzip protoc-3.4.0-linux-x86_64.zip -d protoc

## Download Model:
Only object_detection folder needed:

    svn export https://github.com/tensorflow/models/trunk/object_detection

## Run

    jupyter notebook --ip=0.0.0.0 --port=8080 --no-browser
https://object-detection-eniof.cs50.io/notebooks/object_detection/object_detection_tutorial.ipynb  
* `Cell - Run All`

## Tensorflow Performance

https://github.com/EN10/TensorFlow-For-Poets#performance
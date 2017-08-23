# Object Detection

Based on: 
* [Tensorflow Object Detection API](https://github.com/tensorflow/models/tree/master/object_detection)
* [Installation](https://github.com/tensorflow/models/blob/master/object_detection/g3doc/installation.md)

## Install Tensorflow:

    sudo pip install -U pip  
    sudo pip install tensorflow 
    
## Install dependencies 

    sudo pip install pillow
    sudo pip install lxml
    
Can run without jupyter or matplotlib see below
    
    sudo pip install jupyter
    sudo pip install matplotlib

https://github.com/EN10/MNIST/blob/master/MoreExamples/installJupyter.txt
    
## Download Model:
Only object_detection folder needed:

    svn export https://github.com/tensorflow/models/trunk/object_detection

Subset of:

    git clone https://github.com/tensorflow/models.git
    
## Install Protobuf 2.6+
Download newer binary as Ubuntu 14.04 has 2.5

    wget https://github.com/google/protobuf/releases/download/v3.4.0/protoc-3.4.0-linux-x86_64.zip
    unzip protoc-3.4.0-linux-x86_64.zip -d protoc
    sudo mv ./protoc/bin/protoc /usr/bin/protoc
    chmod a+x /usr/bin/protoc
    protoc object_detection/protos/*.proto --python_out=.

## Run in jupyter
    cd object_detection
    jupyter notebook --ip=0.0.0.0 --port=8080 --no-browser
https://object-detection-eniof.cs50.io/notebooks/object_detection_tutorial.ipynb
* `Cell - Run All`

## Run Without jupyter or matplotlib
    
    mv detect.py ./object_detection/detect.py
    cd ./object_detection
    python detect.py
    
## Tensorflow Performance

https://github.com/EN10/TensorFlow-For-Poets#performance
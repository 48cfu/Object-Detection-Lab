# CarND Object Detection Lab

![](assets/clip.gif)

In lab this you will:

* Learn about *MobileNets* and separable depthwise convolutions.
* The SSD (Single Shot Detection) architecture used for object detection
* Use pretrained TensorFlow object detection inference models to detect objects
* Use different architectures and weigh the tradeoffs.
* Apply an object detection pipeline to a video.

Open the notebook and work through it!

### Requirements

Install environment with [Anaconda](https://www.continuum.io/downloads):

```sh
conda env create -f environment.yml
```

Change TensorFlow pip installation from `tensorflow-gpu` to `tensorflow` if you don't have a GPU available.

The environment should be listed via `conda info --envs`:

```sh
# conda environments:
#
carnd-advdl-odlab        /usr/local/anaconda3/envs/carnd-advdl-odlab
root                  *  /usr/local/anaconda3
```

Further documentation on [working with Anaconda environments](https://conda.io/docs/using/envs.html#managing-environments). 

Particularly useful sections:

https://conda.io/docs/using/envs.html#change-environments-activate-deactivate
https://conda.io/docs/using/envs.html#remove-an-environment

### Resources

* TensorFlow object detection [model zoo](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/detection_model_zoo.md)
* [Driving video](https://s3-us-west-1.amazonaws.com/udacity-selfdrivingcar/advanced_deep_learning/driving.mp4)

### Tips
- Some windows users have reported the driving video as playable only in Jupyter Notebook operating in Chrome browser, and not in media player or Jupyter Notebook operating in other browsers.  In contrast the post-segmentation video appears to be operating across players and browsers.

## Docker and GUI
- To activate GUI with X server Windows: https://blogs.msdn.microsoft.com/jamiedalton/2018/05/17/windows-10-docker-gui/ i.e.  Xming X Server, an X11 display server for Microsoft Windows

## If system is not yet configured
Navigate to installation folder using PowerShell and then
- docker images
- docker system prune
- docker build -t 48cfu_nanodegree_gpu .

## After setting up the system run like
Navidate to project folder. With data/, installation/ example/ etc..
- start Xming as administrator
- Fetch your IP address and use it in the next line and add it to file c:\Program Files (x86)\Xming\x0.hosts
- docker run --privileged -it -v ${pwd}:/src -v /tmp/.X11-unix:/tmp/.X11-unix:ro -e DISPLAY=192.168.1.2:0.0 -p 8888:8888 48cfu_nanodegree

## For jupiter notebook
- docker run --privileged -it -v ${pwd}:/src -v /tmp/.X11-unix:/tmp/.X11-unix:ro -e DISPLAY=$DISPLAY -p 8888:8888 48cfu_nanodegree
- ../run.sh


## TENSOR FLOW
To activate this environment, use:
- source activate carnd-term1

To deactivate an active environment, use:
- source deactivate


## HELP
- https://stackoverflow.com/questions/35595766/matplotlib-line-magic-causes-syntaxerror-in-python-script7
- https://askubuntu.com/questions/685017/how-to-install-nvidia-smi
- https://developer.nvidia.com/cuda-80-ga2-download-archive

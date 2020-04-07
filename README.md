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

### Running with Docker
If you have already installed the [CarND Term1 Starter Kit](https://github.com/udacity/CarND-Term1-Starter-Kit/blob/master/README.md) you should be good to go!   If not, you should install the starter kit to get started on this project.

If you're using `Windows PowerShell`:

```sh
docker run -it --rm --entrypoint "/run.sh" -p 8888:8888 -v ${pwd}:/src udacity/carnd-term1-starter-kit
```

If you're using `bash` or Docker Quickstart Terminal:

```sh
docker run -it --rm --entrypoint "/run.sh" -p 8888:8888 -v `pwd`:/src udacity/carnd-term1-starter-kit
```

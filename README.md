# Lane Line Detection (Term 1 - Project 1)
[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)

<img src="laneLines_thirdPass.jpg" width="480" alt="Combined Image" />

When we drive, we use our eyes to decide where to go. The lines on the road that show us where the lanes are act as our constant reference for where to steer the vehicle. Naturally, one of the first things we would like to do in developing a self-driving car is to automatically detect lane lines using an algorithm.

This repository contains my work and progress for completing this Project succesfully. I've edited this `README.md` file to reflect my comments (please refer to the original README from the forked repository, or in the `ref/` folder of this repository).

## Pipeline Workflow

The Python notebook implementes a series of functions that should be called in the *pipeline* in order to batch process a set of image and video files and produce an output. The workflow I currently have is:

* **Step 0**: open the image
* **Step 1**: output image grayscale
* **Step 2**: Gaussian blur
* **Step 3**: Canny edge processing
* **Step 4**: region masking
* **Step 5**: Hough transformation
* **Step 6**: Weighted image output

## Known issues/bugs

*(2017/03)*

Pipeline rewritten due to error detection after a succesful fix in local environment. Commiting work in progress to preserve history.

*(2016/12/18)*

The process is not working as expected, with a high non-detection rate. I need to tweak the paremeters used and rethink the pipeline. This [GIF](https://gtoran.github.io/repository-assets/udacity-sdcnd-t1p1-lane-line-detection/first-try-lane-detection-error.gif) shows the erroneous behavior.

## DISCLAIMER

This implementation is far from perfect, and usage in a production environment (i.e. autonomous system on a real car with real traffic) is **highly discouraged**.
# **Finding Lane Lines on the Road** 

## Writeup Template

### You can use this file as a template for your writeup if you want to submit it as a markdown file. But feel free to use some other method and submit a pdf if you prefer.

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"

---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

The pipeline to process an image consisted of the following steps - 

1. Conver the image to gray scale.
2. Apply a smoothing function i.e Gaussian Blur
3.Apply Canny algorithm for Edge Detection 
4.Mark Region of interest using pixel co-ordinates
5. Apply hough function to convert to hough space and detect the line coordinates that receive maximum votes
5. Apply weights to reduce error.

![alt text][image1]


### 2. Identify potential shortcomings with your current pipeline

Shortcomings - 

Pixel co-ordinates are static and hard code. Need a more dynamic way to mark region of interest.


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to ...

Another potential improvement could be to ...

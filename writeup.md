# **Finding Lane Lines on the Road** 

---

#### The goal of this project is to make a pipeline that finds lane lines on the road. 

----------
![](https://i.imgur.com/HFS7vP0.jpg)

#### 1. Pipeline description
My pipeline consists of 5 steps.  First, I converted the images to grayscale, then I  continue with the "gaussian blur".  Second, I used the "canny transform" to detect the edge information of the images.  Third, I set a region as the mask.  Fourth, I detected the line segment through "hough transform" in the region.  The last, in order to draw a single line on the left and right lanes, I modified the draw_lines() function by "least squares".

![](https://i.imgur.com/1GReawP.jpg)

### 2. Shortcomings

One potential shortcoming would be what would happen when the ambient light interference is too large, the lane line that meets the requirements will not be detected

Another shortcoming could be the algorithm only applies to straight lanes, and it can't detect curved lane lines.

### 3.  Possible improvements

A possible improvement would be to use multiple curve fitting to accommodate curved lanes.

Another potential improvement could be to use a vehicle-road collaboration system. The lane line is detected by placing a sensor on the lane line.

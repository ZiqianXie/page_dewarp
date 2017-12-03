page_dewarp
===========

Page dewarping and thresholding using a "cubic sheet" model - see full writeup at <https://mzucker.github.io/2016/08/15/page-dewarping.html>

Add horizontal correction based on the derivative of the cubic curve.
TODO: Use symbolic method to get the derivative of the point projection process to speed up the optimization.

Requirements:

 - scipy
 - OpenCV 3.0 or greater
 - Image module from PIL or Pillow
 - Theano
 
Usage:

    page_dewarp.py IMAGE1 [IMAGE2 ...]

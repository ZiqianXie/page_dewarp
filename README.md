page_dewarp
===========

Page dewarping and thresholding using a "cubic sheet" model - see full writeup at <https://mzucker.github.io/2016/08/15/page-dewarping.html>

My modification:

Add horizontal correction based on the derivative of the estimated cubic curve.

Rewrite the projection and objective function using Autograd so that the derivative of the objective function w.r.t the parameters could be calculated. Switching the optimization method from "Powell" to "L-BFGS-B" or "TNC" gets 10x speed-up.

Requirements:

 - scipy
 - OpenCV 3.0 or greater
 - Image module from PIL or Pillow
 - Autograd
 
Usage:

    page_dewarp.py IMAGE1 [IMAGE2 ...]

# ANPR-using-Morhological-maths and Image Enhancement Techniques.
## Technologies used:
 - Python 2.7
 - OpenCv 
## Description :
 Usually Automatic number plate recognition is done using Tesseract and other Techniques. In This code, I have tried to use an another efficient way for number plate recognition. 
 ### The steps that are followed for solving this problem are as follows:
 Image Acquisition.
 RGB to grayscale conversion.
 Noise removal by Iterative Bilateral Filtering(this will preserve the edges while removing the
noise component in the image)
 Contrast enhancement by using Histogram Equalization.
 Morphological opening and image subtraction operation.
 Image binarization or Image Thresholding.
 Edge detection by Canny operator
 Candidate plate area detection by contour detection.
In this step, I found the total contours in the image and sorted all those contours in the
decreasing order based on the contour area. So definitely the number plate contour will appear
in the top 10 or 15 contours in sorted order as number plate will have a contribution of at least
10 percent of the total area of the image.
 Actual number plate area extraction by Masking.
 Enhancement of Extracted plate region by Histogram equalization.
This algorithm worked fine for most of the images that I took. As an answer I tried many cars which are
having different colors (red, blue, black, white, gray) and also with the cars in which the number plate is
inclined in different directions.

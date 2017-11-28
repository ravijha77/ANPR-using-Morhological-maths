# ANPR-using-Morhological-maths and Image Enhancement Techniques.
## Technologies used:
 - Python 2.7
 - OpenCv 
## Description :
 Usually Automatic number plate recognition is done using Tesseract and other Techniques. In This code, I have tried to use an another efficient way for number plate recognition. 
 ### The steps that are followed for solving this problem are as follows:
1. Image Acquisition.
2. RGB to grayscale conversion.
3. Noise removal by Iterative Bilateral Filtering(this will preserve the edges while removing the
noise component in the image)
4. Contrast enhancement by using Histogram Equalization.
5. Morphological opening and image subtraction operation.
6.Image binarization or Image Thresholding.
7.Edge detection by Canny operator
8.Candidate plate area detection by contour detection.
In this step, I found the total contours in the image and sorted all those contours in the
decreasing order based on the contour area. So definitely the number plate contour will appear
in the top 10 or 15 contours in sorted order as number plate will have a contribution of at least
10 percent of the total area of the image.
9. Actual number plate area extraction by Masking.
10.Enhancement of Extracted plate region by Histogram equalization.
This algorithm worked fine for most of the images that I took. As an answer I tried many cars which are
having different colors (red, blue, black, white, gray) and also with the cars in which the number plate is
inclined in different directions.

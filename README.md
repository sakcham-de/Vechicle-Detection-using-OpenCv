# Vehicle Detection

This is a simple Python script is used for vehicle detection using OpenCv and numpy

The script uses the following libraries:
- PIL: For opening and manipulating the image.
- cv2: For displaying the image and converting it to grayscale.
- numpy: For converting the image to a numpy array.
- requests: For downloading the image from the URL.

## How it works

1. The script first downloads an image from a specified URL using the `requests` library.
2. The downloaded image is opened using the `PIL` library's `Image.open()` function.
3. The image is then resized to a dimension of 450x250 pixels using the `resize()` function.
4. The resized image is converted to a numpy array using the `numpy.array()` function.
5. The numpy array is displayed as an image using the `cv2.imshow()` function.
6. The array is then blurred using the Gaussian blur function.
7. After blurring, dilation was applied to the blurred image.
8. After that morphological closing was applied.
9. A classifier named Haar cascade classifier was used which is a opensource classifiers for cars. The classifer was taken from https://gist.github.com/199995/37e1e0af2bf8965e8058a9dfa3285bc6.
10. Rectangular boxes were created around each detected vehicle and shown as output. 



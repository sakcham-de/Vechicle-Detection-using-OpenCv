# Vehicle Detection

This Python script is used for downloading an image from a URL and processing it for vehicle detection.

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
6. The script waits for any key to be pressed before closing the displayed image window using `cv2.waitKey(0)` and `cv2.destroyAllWindows()`.

The script is currently set up to convert the image to grayscale, but this part of the code is not yet implemented.

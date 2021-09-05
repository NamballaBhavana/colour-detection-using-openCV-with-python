# colour-detection-using-openCV-with-python
or a robot to visualize the environment, along with the object detection, detection of its color in real-time is also very important.  Why this is important? : Some Real-world Applications In self-driving car, to detect the traffic signals. Multiple color detection is used in some industrial robots, to performing pick-and-place task in separating different colored objects. This is an implementation of detecting multiple colors (here, only red, green and blue colors have been considered) in real-time using Python programming language. Python Libraries Used:  NumPy OpenCV-Python Work Flow Description: Step 1: Input: Capture video through webcam. Step 2: Read the video stream in image frames. Step 3: Convert the imageFrame in BGR(RGB color space represented as three matrices of red, green and blue with integer values from 0 to 255) to HSV(hue-saturation-value) color space. Hue describes a color in terms of saturation , represents the amount of gray color in that color and value describes the brightness or intensity of the color. This can be represented as three matrices in the range of 0-179, 0-255 and 0-255 respectively. Step 4: Define the range of each color and create the corresponding mask. Step 5: Morphological Transform: Dilation, to remove noises from the images. Step 6: bitwise_and between the image frame and mask is performed to specificaly detect that particular color and discrad others. Step 7: Create contour for the individual colors to display the detected colored region distinguishly. Step 8: Output: Detection of the colors in real-time.

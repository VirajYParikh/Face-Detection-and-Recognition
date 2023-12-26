# Face-Detection-and-Recognition
Basic Implementation of Face Detection and Facial Recognition along with some use of Facial Landmarks

Being a curious tech buff as I am, I was very drawn to Computer Vision and the various applications it has. I came across a very interesting Python library: OpenCV

This package has several use cases one of them being FacialRecognition.

I'd like to explain the steps that I undertook while working on this project. 

Step 1: Reading and processing the image

The image processing packages and libraries that we make use of for facial detection and recognition need a specific kind of input. To make the image readable based on the input, we convert the image into a BGR format which ensures compatibility and improves the efficiency of image processing. 

Moreover, to deal with varying lighting conditions and improve the visibility of facial features, we create a Histogram for each BGR channel. They provide a summary of the color and intensity distribution, which can help in differentiating between different faces.

<div align='center'>
<img width="508" alt="Screenshot 2023-12-26 at 11 24 40 AM" src="https://github.com/VirajYParikh/Face-Detection-and-Recognition/assets/67093208/b886b3ff-52d4-40f7-8985-a6954796715d">
</div>

Step 2: Facial Detection

We would like to run the facial recognition algorithm on an image provided there is a face in the frame to start off with. We use the facial detection algorithm to detect how many faces are present in the image if there are any in the first place.

The `face recognition` library provides us with a `face_location` package which generates the the coordinates of the edges of a rectangle within which it has identified a face in the image. 

<div align='center'>
<img width="387" alt="Screenshot 2023-12-26 at 11 28 46 AM" src="https://github.com/VirajYParikh/Face-Detection-and-Recognition/assets/67093208/fc78c07a-4695-4dad-a83c-220846ff6952">
</div>

Other examples: 
<div align='center'>
<img width="611" alt="Screenshot 2023-12-26 at 11 29 11 AM" src="https://github.com/VirajYParikh/Face-Detection-and-Recognition/assets/67093208/8911acef-9617-4f8d-a8cf-d2d6a5448507">
</div>


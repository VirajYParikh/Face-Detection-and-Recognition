# Face-Detection-and-Recognition
Basic Implementation of Face Detection and Facial Recognition along with some use of Facial Landmarks

Being a curious tech buff as I am, I was very drawn to Computer Vision and the various applications it has. I came across a very interesting Python library: OpenCV

This package has several use cases one of them being FacialRecognition. This project demonstrates some of the features we can make use of for real-world purposes. This includes the implementation of surveillance systems, looking for photos from a list of pictures or images of a particular individual, medical scanning and so on. 

I'd like to explain the steps that I undertook while working on this project. 

### Reading and processing the image

The image processing packages and libraries that we make use of for facial detection and recognition need a specific kind of input. To make the image readable based on the input, we convert the image into a BGR format which ensures compatibility and improves the efficiency of image processing. 

Moreover, to deal with varying lighting conditions and improve the visibility of facial features, we create a Histogram for each BGR channel. They provide a summary of the color and intensity distribution, which can help in differentiating between different faces.

<div align='center'>
<img width="508" alt="Screenshot 2023-12-26 at 11 24 40 AM" src="https://github.com/VirajYParikh/Face-Detection-and-Recognition/assets/67093208/b886b3ff-52d4-40f7-8985-a6954796715d">
</div>

### Feature 1: Facial Detection
We would like to run the facial recognition algorithm on an image provided there is a face in the frame to start with. We use the facial detection algorithm to detect how many faces are present in the image if there are any in the first place. 

The `face recognition` library provides us with a `face_location` package which generates the the coordinates of the edges of a rectangle within which it has identified a face in the image. 

<div align='center'>
<img width="387" alt="Screenshot 2023-12-26 at 11 28 46 AM" src="https://github.com/VirajYParikh/Face-Detection-and-Recognition/assets/67093208/fc78c07a-4695-4dad-a83c-220846ff6952">
</div>

Other examples: 
<div align='center'>
<img width="611" alt="Screenshot 2023-12-26 at 11 29 11 AM" src="https://github.com/VirajYParikh/Face-Detection-and-Recognition/assets/67093208/8911acef-9617-4f8d-a8cf-d2d6a5448507">
</div>

### Feature 2: Facial Recognition
I now  make use of the `face_encoding` package which involves sub-processes:
- Facial Encoding: Facial encoding in the context of facial recognition technology refers to the process of converting facial features from an image into a numerical representation, often called a "facial signature" or "facial feature vector." This process is central to modern facial recognition systems, especially those using machine learning and artificial intelligence.

- Facial encoding starts with detecting and extracting key features from a face in an image. These features typically include elements like the eyes, nose, mouth, jawline, and other distinguishing characteristics.

- The extracted features are converted into a numerical form, creating a feature vector. This vector represents the unique aspects of the face in a way that can be easily processed and compared by computers.

-  The facial encoding allows for easy comparison between different faces. When a new image is presented to the system, it's encoded in the same way, and its feature vector is compared to those in a database.

So here we are encoding the features of the face and uploading them in a database using which we will compare the input images in the system. 

<div align='center'>
<img width="359" alt="Screenshot 2023-12-26 at 11 37 45 AM" src="https://github.com/VirajYParikh/Face-Detection-and-Recognition/assets/67093208/a5093c83-1623-40ef-8466-567cb0368634">
</div>

<div align='center'>
<img width="359" alt="Screenshot 2023-12-26 at 11 38 12 AM" src="https://github.com/VirajYParikh/Face-Detection-and-Recognition/assets/67093208/ea8c1693-92eb-4ef7-9be7-ceaaa4ed6ccd">
</div>

### Feature 3: Facial Landmarks:
There are various other features and applications that Open CV and other image processing packages have to offer which can be useful in a variety of ways. Another one of them is identifying the facial landmarks. 

The `face_landmarks` package in the `facial recognition` library provides us with an array of coordinates over which it has identified the facial landmarks we wish to see, e.g., right/ left eyebrows, chin, ear, etc. It generates a locus in one sense. All we have to do is provide it with an image input and the facial feature. 

<div align='center'>
<img width="359" alt="Screenshot 2023-12-26 at 11 52 41 AM" src="https://github.com/VirajYParikh/Face-Detection-and-Recognition/assets/67093208/41acc29a-a579-4c75-a33c-fea5a01aed12">
</div>


## Conclusion:
There are several other important and innovative technologies in the field of computer vision which in today's world has immense scope and worth diving deep into. `Do not stop looking!`



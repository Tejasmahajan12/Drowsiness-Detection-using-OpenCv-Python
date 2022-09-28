# Drowsiness-Detection-using-OpenCv-Python
This project is used to detect human's drowsiness for any given person. Here we check how long a person's eyes have been closed for. If the eyes have been closed for a long period i.e. beyond a certain threshold value, the program will alert the user by playing an alarm sound.

The program contains following 03 files :-
## Files
 - **face_and_eye_detector_single_image.py** - Detects face and eye from a single image.
 Demo-
 
|  ![Test Image](https://github.com/Tejasmahajan12/Drowsiness-Detection/blob/main/test.jpeg)| ![Result Image](https://github.com/Tejasmahajan12/Drowsiness-Detection/blob/main/result_face_detector_single_image.png) |
|---|---|

 - **face_and_eye_detector_webcam_video.py** - Detects face and eye in a webcam feed by user![Webcam Face and Eye Detection](https://github.com/Tejasmahajan12/Drowsiness-Detection/blob/main/webcam_face_eye_detect.png)
 - **drowsiness_detect.py**- This script detects if person is drowsy or not using webcam video feed

> DEMO
![Drowsiness Detection Demo](https://github.com/Tejasmahajan12/Drowsiness-Detection/blob/main/drowsy_detect_demo.webm)
 
 ## Requirements
> 
> IMPORTANT

  Download `shape_predictor_68_face_landmarks.dat.bz2` from [Shape Predictor 68 features](http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2) 
  Extract the file in the project folder using 
  ``bzip2 -dk shape_predictor_68_face_landmarks.dat.bz``


    numpy==1.15.2
    dlib==19.16.0
    pygame==1.9.4
    imutils==0.5.1
    opencv_python==3.4.3.18
    scipy==1.1.0
Use `pip install -r requirements.txt`to install the given requirements.

## Usage

### Detect Face and Eyes in a Single Image
Put your file to be detected in **images** folder with name **test.jpeg** or change the file path in `Line : 14 face_and_eye_detector_single_image.py` to your image file.
Run script using:

    python3 face_and_eye_detector_single_image.py

### Detect Face and Eyes in a Webcam Feed
Run script using:

    python3 face_and_eye_detector_webcam_video.py
### Drowsiness Detection
Run script using:

    python3 drowsiness_detect.py

The algorithm for Eye Aspect Ratio was taken from pyimagesearch.com blog, by Adrian RoseBrock.

Thank You !

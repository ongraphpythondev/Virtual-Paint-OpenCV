# Virtual-Paint-OpenCV

### Install required python libraries used in Virtual Paint : 
> pip install -r requirements.txt
> extra requirement -> pip install mediapipe

### In this Virtual Paint :
> In this project , we are using python's OpenCV for image virtualization and mediapipe for hand tracking 
> we have created a python module name HandTrackingModule.py to use it to track movements of hand.
> this python library mediapipe library created by google and have been already trained over 30000 different hand images.
> it track hand using 21 point in hand.
> we are also using numpy for creating a blank image so that paint color does get affected since video is just images shifting or changing at a certain speed.
> so , we are using mediapipe for hand tracking , Opencv for image/cam capture and control and numpy for creating a blank image.
> this way mediapipe can detect hand point from cam using opencv and that (numpy's + opencv) blank image is where we actually color.
> but after that that blank image in which we colored , we create a gray scale image of that then make a inverison of it and merge it using bitwise and operator with cam image.
> then at last we use bitwise 'or' operator that merge image with painted blank image result is our cam image with our paint color on it.

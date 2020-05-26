# Virtual-Drawing-Borad
In this drawing Board you can wave your pen in the air and draw shapes or write text on live video feed captured through your webcam.
Features:\n
1)Draw shapes or write text by waving your pen in the air on live video
2)Erase specific part you have drawn
3)Clear the enitre Canvas

This is done entirely in opencv

Steps:
1)The Input image is converted to hsv. And using trackbars object detection for pen cap is done and saved in penval.np. 
2)Then each frame is captured and the co-ordinates of the pen cap are found. 
3)They are joined together using the line function in cv2
4)The top left of the screen shows whethe we are using a pen or an eraser.
5)The drawing are done on grayscale images and then there are add with the original frame capurted.
6)In case of eraser a circle is drawn on the grayscale image of radius=20 from the co-ordinates from received from the virtual pen.


Requirements:
1)Opencv
2)Numpy
3)Webcam

Special thanks to the tutorial of learnopencv.com

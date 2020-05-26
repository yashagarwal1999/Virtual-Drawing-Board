# Virtual-Drawing-Board
In this drawing Board you can wave your pen in the air and draw shapes or write text on live video feed captured through your webcam.
Features:<br/>
1)Draw shapes or write text by waving your pen in the air on live video
<br/>2)Erase specific part you have drawn
<br/>3)Clear the enitre Canvas
<br/>
<br/>This is done entirely in opencv
<br/>
<br/>Steps:
<br/>1)The Input image is converted to hsv. And using trackbars object detection for pen cap is done and saved in penval.np. 
<br/>2)Then each frame is captured and the co-ordinates of the pen cap are found. 
<br/>3)They are joined together using the line function in cv2
<br/>4)The top left of the screen shows whethe we are using a pen or an eraser.
<br/>5)The drawing are done on grayscale images and then there are add with the original frame capurted.
<br/>6)In case of eraser a circle is drawn on the grayscale image of radius=20 from the co-ordinates from received from the virtual pen.
<br/>
<br/>
<br/>Requirements:
<br/>1)Opencv
<br/>2)Numpy
<br/>3)Webcam
<br/>
<br/>Special thanks to the tutorial of learnopencv.com

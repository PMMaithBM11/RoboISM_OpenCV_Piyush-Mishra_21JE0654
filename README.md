# RoboISM_OpenCV_Piyush-Mishra_21JE0654

For Aruco images:
Firstly, I Used the predefined dictionary of 5X5 aruco markers for identification of our markers
Creating a list of the markers in order of their corresponding IDs 
Detection of Marker ID of the marker
Relating the marker IDs with the corresponding colur codes(RGB) where they are to be pasted
calculation of angle of rotated aruco marker
Finding the corrected (straight) images by rotating them in opposite to the angles calculated before
Getting the contours present in the image

For original image:
 Ignoring very small contours(if any) 
 Detection of rectangular/square shapes
 Getting the bounding rectangle for the rectangular shapes
 Drawing the contours and filling it inside with black colour
 Calculating the angle of the shapes with respect to their bounding rectangles 
 Resizing the corresponding marker images to fit in the square boxes Ratio of size of square box to the size of aruco marker image
 Using bitwise_or operator on the image img2 and the resized aruco images
 Since the final destinations for the markers is black space, the OR operator enables the display of white spaces of the marker over the destinations
 Finally, I obtained the desired result i.e placement of the markers of corresponding ids in place of the respective coloured square boxes.

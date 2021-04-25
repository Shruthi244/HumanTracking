# HumanTracking
Humans in the video are detected using the method of Object Detection. Motion of humans are tracked using the method of Object Tracking

# Object detection is the detection on every single frame and frame after frame.
# Object tracking does frame-by-frame tracking but keeps the history of where the object is at a time after time.

# LIBRARIES USED:
•	Tensorflow environment
•	sys
•	cv2
•	Tracker
•	Math
•	Opencv version 4.4.0.44

# Human Tracking
Euclidean Distance tracker method is used for tracking the motion of humans in the video.
# The centroid tracking algorithm works by:
1. Accepting bounding box coordinates for each person in every frame (presumably by some object detector).
2. Computing the Euclidean distance between the centroids of the input bounding boxes and the centroids of existing objects that we already have examined.
3. Updating the tracked object centroids to their new centroid locations based on the new centroid with the smallest Euclidean distance.
And if necessary, marking objects as either “disappeared” or deregistering them completely.

# Human tracking is the process of:

1. Taking an initial set of object detections (such as an input set of bounding box coordinates)
2. Creating a unique ID for each of the initial detections
3. And then tracking each of the humans as they move around frames in a video, maintaining the assignment of unique IDs
Furthermore, object tracking allows us to apply a unique ID to each tracked object, making it possible for us to count unique objects in a video. Object tracking is paramount to building a person counter

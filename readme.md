This project was based upon the idea that a constant video feed will be provided to the model and it will recognize objects
in each of the frame and label them in a box if they are found to be "human". However the main problem observed was to be the
uncertainity of the model to detect humans due to less specific training. Some key points :- 

1. The DL model used in this was from the fast r-cnn model from the tensorflow zoo which was trained on COCO Database
2. Due to the general training on Coco database, the model was not trained on complete human images with different poses,
   physiques, angle of camera etc. Which lead to loss in prediction accuracy since the input image it recieves comes from a
   CCTV camera.
3. Another issue is the low hyperparameter optimization(which i hope to perform later)
4. A secondary design issue is that the model has to recieve the camera footage, break it down into a part before it can perform 
   object detection, ideally it should start recognition at the moment it recieves the data feed.
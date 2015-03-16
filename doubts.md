##1. What will be the resulting prediction? as in a video will be given and we have to detect the polyp in the video.
NOw lets break the video into frames and processing each frame for polyp detection.
Within each frame, we have to segment a possible polyp( but segmentation means that we are detecting the polyp???)
Then, feature extraction from what seems to be a possible polyp(say of 50x50),
then, predictive modelling to detect if it is a polyp or not.

###In my opinion:
This entire project is like a plate detection step in ANPR.
We first segment the possible regions out of each frame(all frames together make up the video),
Then, we extract features and normalize the number of them and 
Then, we train our model to predict new polyps. We train with two classes: polyp and no-polyp out of the possible 
polyp segements that segmentation step gives out, of the training images(frames).

Now, how to do the segmentation and feature extraction first of all, if you could provide me with the scripts of
your work on this.

And also, what is the role of the ground truth image in training?
I understand its significance for the testing: To claculate the number of false P and FN to calcuate two metrics and a third metric is for delay in detection.

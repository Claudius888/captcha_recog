# Solution Intro

**The solution combines a CNN and a FC Classifier and achieves pretty good performance (>94%)**. It :
- crops the image around the characters and flips the cropped image (as we want the time dimension to correspond to the width of the image).  
- uses a CNN to extract features from the cropped image.
- reshapes the features to "split" them into 5 time-steps. 
- uses a FC Classifier to predict 5 characters : for each time-step, the output is the probability distribution of a character being at this step.  

# Dhaka-Ai-2020-Team-Dont-Worry-About-It
These are our notebooks and hyperparameters we used for data preprocessing and training YOLO v5 model for the Dhaka Ai Traffic Detection Challenge 2020 where we ranked among the top 10 teams.

We got help in the preprocessing part from our supervisor. He created the preprocessed dataset using all 21 classes mentioned in the competition. However, we changed the number of classes afterwards to reduce misclassification of the rare classes.

In the training notebook, we tried different hyperparameters and trained the network several times with different pre-processed data using different random splits. We achieved good results by ensembling multiple weights that were trained on different datasets.

Model used: YOLO v5

Input: Images of various traffic vehicles found in Dhaka City. The image annotations were provided in xml files. There were 21 different class of vehicles annotated
Output: Images with bounding boxes and prediction of the class of each vehicle along with accuracy for each prediction

Method: We trained the network using different random splits of the dataset. We used different hyperparameters to find the ones with optimal output accuracy. We also added and hand labeled extra images outside of the given dataset for better learning. We applied different augmentations in the images like scale, shear, rotation etc for better generalization on unseen test data. We found better results by ensembling multiple weights that were trained on multiple randomly generated datasets.

Evaluation: The model was evaluated based on the iou threshold, f1 score and accuracy of prediction.

Drawbacks: One of the constraints was that the model wasn’t performing well on the rare classes. We could have provided additional images for that class but we couldn’t due to shortage of time. Another problem was that the model was not generalizing well on night time images because we did not apply any hsv augmentations.

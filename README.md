# Dhaka-Ai-2020-Team-Dont-Worry-About-It
These are our notebooks and hyperparameters we used for data preprocessing and training YOLO v5 model for the Dhaka Ai Traffic Detection Challenge 2020 where we ranked among the top 10 teams.

We got help in the preprocessing part from our supervisor. He created the preprocessed dataset using all 21 classes mentioned in the competition. However, we changed the number of classes afterwards to reduce misclassification of the rare classes.

In the training notebook, we tried different hyperparameters and trained the network several times with different pre-processed data using different random splits. We achieved good results by ensembling multiple weights that were trained on different datasets.

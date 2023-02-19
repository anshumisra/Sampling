# Random Sampling

Random resampling provides a naive technique for rebalancing the class distribution for an imbalanced dataset.
1. Random oversampling duplicates examples from the minority class in the training dataset and can result in overfitting for some models.
2. Random undersampling deletes examples from the majority class and can result in losing information invaluable to a model.

# SMOTE

One approach to addressing imbalanced datasets is to oversample the minority class. The simplest approach involves duplicating examples in the minority class, although these examples don’t add any new information to the model. Instead, new examples can be synthesized from the existing examples. This is a type of data augmentation for the minority class and is referred to as the Synthetic Minority Oversampling Technique, or SMOTE for short.

# TOMEK LINKS

Tomek Links is one of a modification from Condensed Nearest Neighbors (CNN, not to be confused with Convolutional Neural Network) undersampling technique that is developed by Tomek (1976). Unlike the CNN method that are only randomly select the samples with its k nearest neighbors from the majority class that wants to be removed, the Tomek Links method uses the rule to selects the pair of observation (say, a and b) that are fulfilled these properties:

The observation a’s nearest neighbor is b.
The observation b’s nearest neighbor is a.
Observation a and b belong to a different class. That is, a and b belong to the minority and majority class (or vice versa), respectively.

# NEAR MISS

NearMiss is an under-sampling technique. It aims to balance class distribution by randomly eliminating majority class examples. When instances of two different classes are very close to each other, we remove the instances of the majority class to increase the spaces between the two classes. This helps in the classification process.
To prevent problem of information loss in most under-sampling techniques, near-neighbor methods are widely used.


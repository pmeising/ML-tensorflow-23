# Literature Review

## Overview

Phytoplankton are the foundation in life in aquatic systems.  Rapid responses to changes make them valuable for ecosystem assessment. Different species dominate in different ecosystems. Characterising and quantying species is therefore of great importance. Standard methods, such as taxonomic identification tend to be accuarate but very slow and require trained specialist. The advancement of identification technology, such as imageing flow cytometrs, has lead to more rapid imaging. However, the immense amount of data has been proven challenging to analyse. In the last years, Deep Meaching Learning algorithms, such as Convolutional Neural Networks (CNNs) have helped with the idenfication process. All images were resized to 180x180 pixels. 

Source [1]
The study by [1], used pre-trained ResNet-18 CNN with 18 layers from TorchVision -  a large PyTorch project.  This model, pre-trained on RGB images with 1000 classes, aimed to enhance performance on unseen images and mitigate overfitting and class imbalances. Random oversampling addressed underrepresented phytoplankton classes, accompanied by image augmentations (e.g., rotations, zoom, brightness changes) for all classes in the training data. Model training employed categorical cross-entropy loss with the Adam optimizer and a custom learning rate schedule, featuring three steps progressively adjusting trainable layers and learning rates. Evaluation metrics included class-specific measures like recall, precision, and F1-score, with a weighted average F1-score chosen to handle class imbalance and operational considerations.

Additionally, a filtering method was implemented for the deployed CNN to address unclassifiable images captured by the Imaging FlowCytobot (IFCB). This involved using class-specific probability thresholds determined through evaluation on the Validation Data. The final CNN layer incorporated a scaling factor to enhance smoothness in class probabilities, aiding in the establishment of effective thresholds for image classification.

This project milestone requires you to review the literature related to your project. The objective is to gain a deeper understanding of the problem domain, as well as to identify similar approaches or solutions that have been tried before.
You might want to answer the following questions:
  * Which are the models commonly used for my problem?
  * Which format must the training data have?
  * How much training data is typically used in similar problems?
  * Are there pretrained models I can use for my problem?

## Guidelines

1. **Minimum Number of Sources**: You are required to review at least two or three papers, blogs, or authoritative sources related to your project topic.

1. **Summary**: For each work, provide a brief summary that includes the objective of the work, methods used, and the outcomes. One sentence on each point is sufficient.

## Submission

Complete the template provided in the [README](README.md) of this folder.

# Phytoplankton Classification

## Repository Link

[Link to this repository](https://github.com/pmeising/ML-tensorflow-23/tree/main?tab=readme-ov-file)

## Description

This project aims to develop a sophisticated Convolutional Neural Network (CNN) for the classification of a diverse set of phytoplankton, leveraging a dataset of approximately 63,000 labeled images spanning 50 distinct classes. The objective is to refine the accuracy of phytoplankton classification, enhancing understanding of their distribution and ecological roles. By employing advanced machine learning techniques and a substantial image dataset, the project seeks to overcome challenges in species identification due to morphological similarities

### Task Type

Multiclass Image Classification Problem

### Results Summary

- **Best Model:** [MobileNetV2 based model_30_39.h5](3_Model/Models/model_30_39_175_1.h5)
- **Evaluation Metric:** Weighted Average F1-Score, Macro Average F1-Score
- **Result:** 97%, 99%

## Documentation

1. **[Literature Review](0_LiteratureReview/LiteratureReview.md)**
2. **[Dataset Characteristics](1_DatasetCharacteristics/exploratory_data_analysis.ipynb)**
3. **[Baseline Model](2_BaselineModel/baseline_model.ipynb)**
4. **[Model Definition and Evaluation](3_Model/model_definition_evaluation.ipynb)**
5. **[Presentation](4_Presentation/Phytoplankton_Image_Classification.pdf)**

## Cover Image

![Project Cover Image](CoverImage/Cover_image_phytoplankton.png)


##Version 2

In version 2 I train a model on a MobileNetV2 CNN and thereby extract the features of the different Phytoplankton. Instead of the blind split that was done in the previous attempt of version 1, here the split is made based on the extractable features. The goal is to train a model that is capable of identifying the most classes possible out of the 50. The model selected 30 out of the 50 classes and reaches an average weighted F1 Score of 94%.

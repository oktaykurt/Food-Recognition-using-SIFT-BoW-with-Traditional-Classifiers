# Food Recognition using SIFT/BoW with Traditional Classifiers

This repository contains the implementation of a traditional machine learning approach using Scale-Invariant Feature Transform (SIFT) and Bag of Words (BoW) representation with Support Vector Machines (SVM) for food recognition. The dataset used for this project is the iFood-2019-FGVC6 dataset, which comprises 251 food classes.

## Repository Contents

- **Swift and BoW Technique**: This folder contains the code and implementation details for the SIFT and BoW techniques.
- **Notebooks**: Jupyter notebooks used for data preprocessing, feature extraction, and model evaluation.
- **Data**: Scripts to handle and preprocess the iFood-2019-FGVC6 dataset.

## Project Overview

This project aims to develop and evaluate two approaches for food recognition:
1. A Convolutional Neural Network (CNN) approach.
2. A traditional machine learning approach using SIFT and BoW with SVM.

**Note**: The CNN model is not included in this repository due to its limitations and is discussed in the associated research paper.

## Data Preprocessing

Data preprocessing steps included:
1. Unzipping and reading the dataset.
2. Splitting the dataset into training and validation sets.
3. Image augmentation (for CNN).
4. Image resizing and normalization.
5. Efficient data handling to manage the large dataset size.

## Model Architecture and Training

### SIFT/BoW with SVM

- **Feature Extraction**: Using SIFT to extract keypoints and descriptors from the images.
- **BoW Representation**: Converting SIFT descriptors into a histogram representation using the Bag of Words model.
- **Classification**: Using Support Vector Machines (SVM) with both linear and RBF kernels to classify the BoW histograms.

## Evaluation

The performance of the models was evaluated on validation and test sets. Key metrics include accuracy, precision, recall, and F1 score.

## Results

- **SVM with RBF Kernel**: Showed better performance compared to the linear kernel.
- **Challenges**: Handling a large dataset with computational constraints was a significant challenge.

## Future Work

- Enhance the CNN architecture for better performance.
- Explore advanced feature extraction techniques.
- Implement sophisticated data augmentation and preprocessing methods.

## Research Paper

The detailed findings and methodologies are documented in the research paper:

**Food Recognition using CNNs and SIFT/BoW with Traditional Classifiers**  
_Oktay Kurt_  
Department of Artificial Intelligence for Science and Technology, University of Milano-Bicocca, Milan, Italy  
o.kurt@campus.unimib.it

**Abstract**: This project develops and evaluates two approaches for food recognition: a CNN and a traditional machine learning approach using SIFT and BoW with SVM. The dataset comprises 251 food classes with varying image counts. Despite computational constraints and dataset size, the project provides insights into the challenges and potential improvements for food recognition systems.

You can download the full research paper [here](./Food Recognition using CNNs and SIFT/BoW with Traditional Classifiers.pdf).

## Citation

If you use this code in your research, please cite the paper:

@inproceedings{foodrecognition2024,
title={Food Recognition using CNNs and SIFT/BoW with Traditional Classifiers},
author={Kurt, Oktay},
booktitle={Proceedings of the International Conference on Artificial Intelligence},
year={2024},
organization={University of Milano-Bicocca}
}

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

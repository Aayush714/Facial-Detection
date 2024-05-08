Machine Learning Approach for Spontaneous Facial Expression Recognition


Overview 

This project leverages machine learning to identify facial Action Units (AUs) from image data. It employs a variety of feature extraction techniques and classifiers to evaluate and compare their effectiveness in detecting AUs.


Processing Pipeline
The project consists of several Jupyter notebooks, each performing specific tasks in the data processing and feature extraction pipeline:

1. Preprocessing_data.ipynb
This notebook handles initial data preprocessing steps. It includes loading and cleaning data, normalizing images, and preparing them for feature extraction processes.

2. Combined_Gabor.ipynb
This notebook focuses on the extraction of Gabor features from the preprocessed images. It applies Gabor filters to capture texture information which is crucial for recognizing facial AUs.

3. Compute_HOG.ipynb
This notebook is dedicated to calculating Histogram of Oriented Gradients (HOG) features. HOG is critical for capturing edge or gradient structures that is characteristic of local shape, which is useful for AU detection.

4. Combined_HOG&Gabor.ipynb
The final notebook in the sequence, combines the features extracted from both the Gabor and HOG methods. It then applies multiple machine learning classifiers to these combined features to detect and classify the facial AUs.

Usage
Follow the notebooks in the sequence provided above to ensure all features are correctly generated and utilized by the classifiers.

Requirements
To run the notebooks, include all the necessary libraries to ensure compatibility and functionality across all processing and analysis steps.
numpy
scikit-learn
scikit-image
tqdm
matplotlib
seaborn
opencv-python-headless
imblearn
tensorflow
pandas
json
pickle
dlib

Testing 
During testing, we found Subject 9 getting out of the frame, so we did not compute Subject 9 (SN009) in our features. Also, for the combined HOG&Gabor, the computation time to run was too high so random subjects were selected. 

Contribution 
The project was collaboratively developed with equal contributions from both team members, ensuring a comprehensive approach to the problem and solution development.


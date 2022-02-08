# Automated Classification System for Tick-Bite Defect on Leather

A six-step preprocessing procedure is introduced to enhance the quality of the leather image in terms of visibility and to preserve important features representation. Then, multiple classifiers are utilized to differentiate between defective and nondefective leather patches.
 
Example of leather patches:

<img src="https://github.com/christy1206/XBoost-ANN/blob/picture/leather.JPG" width="600" height="300"/>

The recognition results achieved are:

<img src="https://github.com/christy1206/XBoost-ANN/blob/picture/result.JPG" width="600" height="450"/>

The pre-processing techniques involved are:
1) histogram matching - *imhistmatch(I,ref)*
2) resizing - *imresize(I,[100 100])*
3) grayscale normalization *rgb2gray(I)*
4) Gaussian blurring - *imgaussfilt(I)*
5) Canny edge detection - *edge(I,'canny')*

The feature extractor involved is:
1) Histogram of Gradient *extractHOGFeatures(I)*

The classifers involved are (using Classification Learner App in MATLAB):
1) k-NN 
2) SVC 
3) SVM 
4) AdaBoost
5) Random Forest
6) Discriminant Analysis
7) Extreme gradient boosting

The databases include two types of leather patches: with tick bite defects and non-defective images.

## Matlab code
Software is written and tested using Matlab 2020b, toolbox required:
1) Parallel Computing Toolbox 
2) Computer Vision System Toolbox
3) Statistics and Machine Learning Toolbox


## If you use this method in your research, please cite:

@inproceedings{liong2022automated,\
  title={Automated Classification System for Tick Bite Defect on Leather},\
  author={Y.S. Gan, Wei-Chuen Yau, Sze-Teng Liong, Chih-Cheng Chen},\
  journal={Mathematical Problems in Engineering},
  year={2022}
}

If you have suggestions or questions regarding this method, please reach out to stliong@fcu.edu.tw

Thank you for your interest and support.

## Introduction
Given that there are limited COVID-19 testing kits, we need to rely on other diagnosis measures. For the purposes of this project, we thought to explore X-ray images as doctors frequently use X-rays and CT scans to diagnose pneumonia, lung inflammation, abscesses, and/or enlarged lymph nodes.
Since COVID-19 attacks the epithelial cells that line our respiratory tract, we can use X-rays to analyze the health of a patient’s lungs, and given that nearly all hospitals have X-ray imaging machines, it could be possible to use X-rays to test for COVID-19 without the dedicated test kits.


## Implementation
So, for the project we used the TensorFlow 2.0 and Keras deep learning libraries via a selection of tensorflow.keras imports.
Additionally, we use scikit-learn, the de facto Python library for machine learning, matplotlib for plotting, and OpenCV for loading and preprocessing images in the dataset. VGGNet architecture has been used to build the model. 
The datasets have been prepared by compiling images from many other open-source datasets. The folder '''dataset_new''' is the prepared dataset. The other two folders are snipped from the '''dataset_new''' folder for testing purposes.
There are two prepared models, each using a different optimization method.
Hierarchy of the dataset :
├── dataset
│   ├── covid 
│   └── normal

There is also a python script for the second model '''CXR_model2'''.
Usage of the script is as follows :
'''python cxr_covid_model_2.py --dataset <path to dataset>''' ; for example '''python cxr_covid_model_2.py --dataset dataset_new_test'''.
  Important - hierarchy of the input dataset should be of the above mentioned format.

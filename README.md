# Machine-Learning_Engineer-Nanodegree
## Capstone Project for Udacity's Machine Learning Engineer Nanodegree Program

The proposal for the capstone project for the Machine-Learning Engineer Nanodegree course is described in proposal.pdf.

The relevant dataset (X-ray images) can be acquired from the Kaggle through the link below:

https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia

This capstone project to complete the Udacity's Data Science Nanodegree Program. 

## Table of Contents

1. [Project Motivation](#project_motivation)
2. [Files Descriptions](#files_descriptions)
3. [Python Libraries](#python_libraries)
4. [Results Summary](#results_summary)
5. [License](#license)
6. [Acknowledgement](#acknowledgement)

<a name="project_motivation"></a>
## Project Motivation
This is a capstone project to complete the Udacity's Machine Learning Nanodegree Program. In this project, the chest X-ray data from the Kaggle is used to build the models that can instantly classify a chest X-ray into the normal or the one with pneumonia. The description of the entire process adopted can be found in the file   **Project_Report_MLED.pdf**.

<a name="files_descriptions"></a>
## Files Descriptions

The enitre process adopted are carried out in the following one notebook.
    
        1.  medical_diagnosis.ipynb: Data exploration, preprossing, and model traing/testing/predictions are carried out in this notebook.
        
        The data files are explained in details in the notebooks as well as in the Project_Report_MLED.pdf file.

Step-by-step description of the entire process adopted in the project is explained in the file **Project_Report_MLED.pdf**.

<a name="python_libraries"></a>
## Python Libraries

The following python libraries are required to run the notebooks:
        
	> Pandas
	> Numpy
	> Scikit-learn
	> Keras
	> TensorFlow
	> Matplotlib
	> Seaborn

	
<a name="results_summary"></a>
## Results Summary

I have tried the following three models and considered the model **accuracy** score and F1-score as the metric to evaluate the model quality.

    i. Convolutional Neural Netwrok (CNN): This model is considered as a benchmark and all the other models’ performance is compared with it.
    ii. Transfer Learning Model using VGG19 pre-trained model (TL-VGG19)
    iii. Transfer Learning Model using ResNet152 pre-trained model (TL-ResNet152)

All the three models mentioned above are trained on the training set and evaluated on the testing set. The size of the training set is 5218 and the testing set is 624. The models’ accuracies and F1-score are compared.

The benchmark model **CNN** has a training and testing accuracy of 95.07% and 77.04%, respectively. The **TL-VGG19** model has a training accuracy of 84.22% and a testing accuracy of 65.22%. Similarly, **TL-ResNet152** model has the training and testing accuracy of 92.14% and 85.26%, respectively. 

Out of three models, I have confirmed the **TL-ResNet152** as the best classifier because of its better testing accuracy and F1-score. 

For the nature of the problem chosen and the given data sets, we are convinced that the final model reached a good accuracy which can be improved by expanding the training data sets. 

The details are explained in the file **Project_Report_MLED.pdf**.
<a name="license"></a>
## License
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)


<a name="acknowledgement"></a>
## Acknowledgement
* We want to thank [Udacity](https://www.udacity.com/) for this project and **Kaggle** for the data sets.



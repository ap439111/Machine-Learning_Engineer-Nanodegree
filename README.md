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

I have tried the following five models and considered the model **accuracy** score as the metric to evaluate the model quality.

    i. Neural Network: This model is considered as a benchmark and all the other models’ performance is compared with it.
    ii. Decision Tree Classifie
    iii. K-nearest Neighbor
    iv. Random Forest
    v. Support Vector Machine
	    
The features used in training the models are a reward, difficulty, offer_duration_hrs, BOGO, discount, informational, mobile, social, web, age_group, became_member_on, income, income_group, F, M, N, O.


All the five models mentioned above are trained on the training set and evaluated on the testing set. The size of the training set is 53393 and the testing set is 2284. The models’ accuracies are compared.

The benchmark model **neural network** has a training and testing accuracy of ~64%. **Decision Tree** has a training accuracy of 94.64% and a testing accuracy of 57.77%. Similarly, **K-Nearest Neighbor** has the training and testing accuracy of 68.82% and 61.48%, respectively. **Random Forest** has a training accuracy of 94.64% and a testing accuracy of 59.76%. **Support Vector Machine** has a training accuracy of 60.90% and a testing accuracy of 61.39%.

Out of five models, I have considered Random Forest and K-Nearest for further refinements using the GirdSearchCV. Random Forest has high train accuracy and relatively lower test accuracy. This means the model is behaving differently for the training and testing sets. On the other hand, the K-Nearest Neighbor has both the training and testing accuracy in the same range. 

After refinements, the Random Forest has a training accuracy of 65.40% and a testing accuracy of 64.70%. Thus, the tuned parameters behave in a similar way for both data sets. Similarly, after refinements, the K-Nearest Neighbor has the training and testing accuracy of 73% and 60.8%, respectively. 

Out of the two refined models, I have taken the **Random Forest** as the best classifier because of its better testing accuracy. 

For the nature of the problem chosen and the given data sets, we are convinced that the final model reached a good accuracy. The customers’ behavior for an offer can be varying and that could be a reason for the model to have medium accuracy.

The details are explained in the file **project_capstone.pdf** and a [bolgpost](https://anup-pandey123.medium.com/starbucks-capstone-challenge-4a763b207985).

<a name="license"></a>
## License
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)


<a name="acknowledgement"></a>
## Acknowledgement
* We want to thank [Udacity](https://www.udacity.com/) for this project and **Starbucks** for the data sets.



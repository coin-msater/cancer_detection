# NUS IT1244, AY 2023/24, Sem 2  
## Team 31: CancerStagers

Hello and welcome to our Github repository for our IT1244 project by Nitish Kumar Sahoo, Leong Jing Rou, Wang Ruoyu and Rikhil Singh!

In this repository, we have 8 files (including this README) and 1 folder which contains 2 additional files. A brief overview of the essential files and how to run this project is given below, and by following the instructions, you should be able to run the necessary files smoothly.

## Overview of Contents

### **Requirements**

This text file contains the necessary libraries (as well as the versions used in the code files) to be installed for the code to run successfully. It is strongly advised to check that they have been installed. If you ae unsure of the installation, you can install the libraries by running the `pip install -r requirements.txt` in your command prompt/ terminal. 

### **NUS_IT Folder** 

This folder contains 2 csv files, *Train_Set.csv* and *Test_Set.csv*, which are used for the training and testing of our saved models respectively. So long as the complete folder is downloaded on your computer with the NUS_IT folder being a subfolder alongside the jupyter notebooks (`.ipynb`), the code in those notebooks will run owing to the use of relative paths. 

### **Primary & Secondary Models**

Our group has decided on a hierarchical multi-model approach for enhanced classification of the different stages of cancer - including that of healthy patients. As a result, 2 models are used; a primary model that yields 4 distinct classes as outputs as well as a secondary model that gives binary results. Elaboration on the models can be found in the jupyter notebook IT_Proj - Final_v3, as well as the word document. However, to enable the models we created to be saved and loaded quickly, they were saved in the pickle files *CancerStagersPrimaryModel.pkl* and *CancerStagersSecondaryModel.pkl*. In the event they are absent/ corrupted, they can be made again by running the *IT_Proj - Final_v3.ipynb* notebook, yet with their presence, the evaluation of the saved model performance can be performed much more quickly with the use of the *IT_Proj - Novel.ipynb* notebook instead.

### **Jupyter Notebooks**

This repository contains 3 jupyter notebooks - *IT_Proj - Final_v3.ipynb*, *IT_Proj - Novel.ipynb* and *IT_Proj - Base.ipynb*. The first notebook consists of our group's collective efforts in training the optimal Random Forest and Gradient Boosting models to classify people into different stages of cancer. The second notebook consists of code that looks at the performance of the models when sequenced together on raw data (that we sample from our test set). The last notebook consists of a single baseline Random Forest model that we use as a point of comparison with our hierarchical model in the Final_v3 file to compare our model's performance.

All notebooks can be run, yet owing to the incoportation of training various types of models in the former, the runtime of *IT_Proj - Final_v3.ipynb* is significantly longer - taking about half an hour to run. Furthermore, it does have segments of code that have been placed in multi-line string comments (these parts of code are prefaced with the comment `# takes about 15 - 30 minutes to run`). While these code segments are not supremely vital to be run as their results have been recorded and can be reproducible, the choice to uncomment the code and run it entirely can be done; but will push the runtime of the file to at least an hour. 

For the *IT_Proj - Base.ipynb*, it is of a similar situation that the file's runtime will take at least 20 minutes. Furthermore, with the file mainly just acting as a point of comparison, it does not have to be run. As a result, it is strongly advised to solely run the *IT_Proj - Novel.ipynb* file which you can run to test the performance of models. Indeed, it can also run on newer, unseen data > so long as of course it is a csv file organised similarly to *Test_Set.csv*. An analysis of all files can be conducted if wished however, but the focus should be on the *IT_Proj - Final_v3.ipynb* and *IT_Proj - Novel.ipynb* notebooks.

### **Report**

Our Repository also consists of a report that outlines our research and methodology as well as the advantages and limitations of the approach we have taken. This report, in conjunction with the jupyter notebooks, aims to provide a comprehensive overview on our aims and accomplishments in this insightful project we have engaged in.

# MLDA@EEE Deep Learning Week Hackathon
<br>Dates: 30 Sep 2022 - 3 Oct 2022
<br>Team: The Learners
<br>Team Members: Ian Ng, Josiah Chua, Calvin Wen, Ong Zhi Hong, Alfred Leong
<br>[Submission Link](https://devpost.com/software/tabnet-to-identify-diabetic-patients-at-risk-of-re-admission)

### A TabNet classifier to identify diabetic patients at risk of hospital re-admission
#### Summary
* Implemented a TabNet classifier with an AUC of 0.62 to identify diabetic patients with high risk of readmission so that healthcare practitioners can intervene to reduce their risk factors
* Proof of concept for healthcare institutions to use similar deep learning models to identify at-risk diabetic patients, prompting physician consultations for curation of management plans

The dataset used was the Diabetes 130-US hospitals for years 1999-2008 Data Set. In thinking of which model to use for this identification task of whether a patient is at risk of being re-admitted into hospital, other models we considered were Random Forest Classifiers, Naive Bayes Classifiers or an Ensemble of Decision Tree Classifiers. We ultimately decided on implementing a TabNet (https://arxiv.org/abs/1908.07442), a novel high-performance and interpretable canonical deep tabular data learning architecture, on account of its demonstrated performance beating neural network and decision tree variants for a wide range of tabular datasets.

In this repository, one can find the Diabetes 130-US hospitals for years 1999-2008 Data Set (csv file) used for training our model as well as a mapping of numerical IDs to their categorical equivalents for the ***admission_type_id, discharge_disposition_id and admission_source_id*** variables. This repository also contains our source code for the implementation of TabNet and the associated data wrangling and training of the model, having taken reference from Somshubra Majumdar's (@titu1994) [implementation](https://github.com/titu1994/tf-TabNet).

![This is an image](https://github.com/titu1994/tf-TabNet/blob/master/images/TabNet.png?raw=true)

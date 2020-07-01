# MRNET-for-Knee-Diagnosis
Developed a deep learning model for detecting general abnormalities and specific diagnoses ( [ACL] tears and meniscal tears) on knee MRI exams  . 
Problem Statement 


It's an image classification problem. We want to detect knee injuries from an input MRI scan.
MRI is a kind of rays used in medical diagnosis, where the organ is examined in three planes: sagittal, coronal, and axial planes. For each plane, many slices (pics) are taken for the patient, and this group of slices is called a scan and it has size (s). The three views' scans represent an exam.
We have here three knee injuries that represent the labels or the network outputs (Abnormal, ACL tears, and Meniscus tears). Note that more than one type can be associated with one scan. For example, an MRI scan which is abnormal can also have an ACL tear and so on.
Given three MRI scans in three views(axial, coronal, sagittal), we want to get nine injury probabilities (3 to each view). From them, we can get 3 injury probabilities for the exam itself (3 scans). Every three probabilities of each injury that are coming from the three views should be processed by a logistic regression classifier to get one probability value for this injury. It represents an injury's probability for this exam. Therefore, three logistic regression classifiers can be used.

Applying VGG,INCEPTION,RESNET models  for feature extraction from scratch using Keras.

Use transfer learning state to start with a better set of networks’ weights trained on famous datasets. Here, you will use ImageNet
weights to enhance the training of well-known networks.


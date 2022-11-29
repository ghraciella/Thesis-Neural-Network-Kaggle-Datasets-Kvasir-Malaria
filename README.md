# Thesis-Neural-Network-Kaggle-Datasets-Kvasir-Malaria


<p><h2 align="center"><font color="red"> Abstract </font></h2>

Medical images are not always readily available, it can often be tedious for medical practitioners to not
just collect but annotate and analyze these images especially for multi-class image data. In a bid to reduce the
workload, aid in diagnosis and treatment of diseases we try to implement and understand how articial neural

networks can be used in the automatic classication of these images. The results gotten from the implementa-
tion of the neural network models on our chosen datasets can help in determining how to improve the models

used in training these images.

In this work, we implemented the Fully Connected Neural Network (FCN) and the Convolutional Neural Net-
work (CNN) on the Malaria Cell Images dataset and and Kvasir dataset made available by National Institutes of

Health (NIH), Vestre Viken Health trust and Cancer Registry of Norway (CRN). These medical image datasets
were published on Kaggle for research purposes by data analyst and can also be uploaded by users.
We explore the relevant mathematical background for the various components of the implemented Neural
Network (NN) architectures which are used in computer vision for image classication and the mathematics
behind how the back propagation works in these networks. We also make comparisms of several optimization
algorithms in the keras library and analysed how well they performed on the train and test sets of our chosen

datasets as well as investigate how netuning the hyperparameters of the can aect the models prediction ac-
curacy.

Keywords: Neural Networks; Medical Imaging; Image Classication; Kvasir dataset; Endoscopic Images;
Malaria; Optimization; BackPropagation; Hyperparameter Tuning; Regularization





<p><h2 align="center"><font color="red"> Contents </font></h2>

<ol>
<li>1 Introduction 2</li>
<li>1.1 Motivation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2</li>
<li>1.2 Kaggle Datasets . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2 </li>
<li>1.2.1 Malaria Cell Images Dataset . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2</li>
<li>1.2.2 Kvasir Dataset . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3</li>
<li>1.3 Overview of Project Work . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 5</li>
<li>1.4 Literature review . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 5</li>
<li>2 Topology of the Neural Network Models and Back-Propagation 7</li>
<li>2.1 Fully Connected Neural Network Model . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 7</li>
<li>2.1.1 Initializing The Network Parameters and Forward Propagation . . . . . . . . . . . . . . . 7</li>
<li>2.1.2 Loss Function and Error computation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 8</li>
<li>2.1.3 Back Propagation and Optimization . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 9</li>
<li>2.2 Convolutional Neural Network Model . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 11</li>
<li>2.2.1 Initializing The Network Parameters . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 12</li>
<li>2.2.2 The Convolution Layer + Activation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 12</li>
<li>2.2.3 The Pooling layer . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 13</li>
<li>2.2.4 The Dense layer and Loss . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 13</li>
<li>2.2.5 BackPropagation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 13</li>
<li>2.2.6 Optimization Algorithms . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 15</li>
<li>3 Application on Selected Kaggle Datasets 20</li>
<li>3.1 Analysis for the Malaria dataset . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 20</li>
<li>3.2 Analysis for the Kvasir dataset . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 23</li>
<li>4 Hyperparameter Optimization and Optimization Algorithms Analysis 27</li>
<li>4.1 Results from Hyperparameter Optimization . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 27</li>
<li>4.2 Analysis of Results for the Optimization Algorithms . . . . . . . . . . . . . . . . . . . . . . . . . 33</li>
<li>5 Conclusion 39</li>
<ol>

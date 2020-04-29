# Lung-Disease-Diagnosis-using-X-ray
<b>Using DenseNet to diagnose 14 types of Lungs disease with help of X-Ray images</b>

<b>Dataset:</b> <a href="https://arxiv.org/abs/1705.02315">Chest X-Ray Dataset</a> by Cornell University

<p> Chest X-ray is one of the most important diagnosis tool  for medical. They are critical for detection of pneumonia, lung cancer , mass(damage of tissue) etc. In this project, 14 types of lung disease were detected using chest X-rays</p>
<p><b>Major Challanges working with real work medical data were:</b></p>
<p><b>Class Imbalance-</b> Not an equal number of examples of disease and non disease examples. ex. More examples of Normal condition than of condition with disease , which creates problems for learning algorithm for tracing disease.

Solution: Using weighted loss:Wp and Wn with muli label loss where
Wp = num of negative/total, 
Wn=num of positive/total
OR 
Resampling: Undersampling, Oversamplng</p>

<p><b>Multi Task-</b> Multiple classification task using one model

Solution: Using  different weighted loss for different disease with multi label loss function
</p>

<p><b>Dataset size-</b>Size of datset is small ie.e aroung 1400 images.

Solution: using pretrained model and do transfer learning
OR Data Augmentation(Label may change when we flip images)
</p>

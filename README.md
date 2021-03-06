![banner.jpg](https://github.com/a-woodbury/DeepBreath/blob/master/Resources/deepbreathsplash.jpg)

**Identifying Pneumonia in Chest X-rays using Deep Learning**

### Overview

According to the [American Thoracic Society](https://www.thoracic.org/patients/patient-resources/resources/top-pneumonia-facts.pdf), Pneumonia is the world’s leading cause of death among children under 5 years of age, killing approximately 2,400 children a day causing it to be the number 1 most common reason for US children to be hospitalized. Although we have adequate treatment for it like our oral and IV antibiotics, IV fluids, oxygen and rehydration therapy, we must be able to detect it and treat it immediately to prevent long term complications and death. </br>

In this project, our goal is to train and build a deep learning model that can classify whether a given patient has pneumonia, given a chest x-ray image.

### Repository Navigation
<pre>
Technical Notebook : <a href=https://github.com/a-woodbury/RxVision/blob/master/Notebooks/RxVision_Technical_Notebook.ipynb>Technical Notebook </a>
Other Notebooks    : <a href=https://github.com/a-woodbury/RxVision/blob/master/RxVision_Modeling.ipynb>Modeling</a>, <a href=https://github.com/a-woodbury/RxVision/blob/master/RRxVision_Data_Collection.ipynb>Data Collection Notebook </a>
Dataset Links      : <a href=https://www.nlm.nih.gov/databases/download/pill_image.html>NIH RxImage Portal</a>, <a href=Link>GCP Bucket</a>
Presentation       : <a href=https://github.com/a-woodbury/RxVision/blob/master/Presentation/RxVision.pdf>Slide Deck</a>, <a href=https://docs.google.com/presentation/d/1f2bLza9GFhIXUAMudNsb00RTpHAwg5JegGIw2i2Jg8A/edit?usp=sharing>Google Slides</a>
Other              : <a href=Link>Recreating the Model Guide</a>, <a href=Link>Drug Classes</a>
</pre>

### ReadME Navigation

[Problem](https://github.com/a-woodbury/RxVision/blob/master/README.md#problem) - 
[Data](https://github.com/a-woodbury/RxVision#data) -
[Model](https://github.com/a-woodbury/RxVision#model) -
[Results](https://github.com/a-woodbury/RxVision#results) - 
[Recommendations](https://github.com/a-woodbury/RxVision#recommendations) - 
[Future](https://github.com/a-woodbury/RxVision#future) - 
[Project Info](https://github.com/a-woodbury/RxVision#project-info) -
[Works Cited](https://github.com/a-woodbury/RxVision#works-cited)


![coverphoto.png](https://github.com/viviandng/flatiron-project-4/blob/master/images/xray.png)

</pre>

## Problem

**Method**
1.	Download the dataset 
2.	Reshape x-rays to  64x64 and create a baseline model with dense layers (fully connected)
3.	Train the data on different models and compare recall scores
    - Densely Connected Neural Network
    - Convolutional Neural Network
    - DenseNet Pretrained
4.	Test the data on the best model (highest recall score)


## Data
<pre>
Dataset Links    : <a href=https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia>Chest X-Ray Images (Pneumonia) Dataset (Kaggle)</a>
                 : <a href=https://data.mendeley.com/datasets/rscbjbr9sj/2>Chest X-Ray Images (Pneumonia) Dataset (Original Dataset)</a>
</pre>



https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia

- Train folder:
  - 1341 normal 
  - 3875 pneumonia 
- Val folder:
  - 8 normal 
  - 8 pneumonia 
- Test folder:
  - 234 normal 
  - 390 pneumonia 

## Model


## Results

Model | Accuracy | Precision | F1 | **Recall** |
--- | :---: | :---: | :---: | :---: |
Baseline Dense | 0.81 | - | - | n/a
CNN | - | 0.93 | 0.88 - | 0.9
DenseNet | 0.61 | 0.62 | 0.76 | 0.98



### Recommendations:

- Incorporate our model to IT softwares (ex: epic) in hospital settings to assist health professionals diagnose pneumonia patients
- Use our model under the supervision of a radiologist to enhance accuracy/recall to improve treatment outcomes which will increase hospitals' ratings and fundings. 

## Future

- Improve the current model with additional chest x-ray data from adult patients 
- Explore machine learning solutions that detects the cause of pneumonia (viral vs bacterial)


## Project Info

<pre>
Contributors : <a href=https://github.com/a-woodbury>Alphonso Woodbury</a>
               <a href=https://github.com/viviandng>Vivian Dang</a>
</pre>

<pre>
Languages    : Python
Tools/IDE    : Anaconda, Colab
Libraries    : Tensorflow, Keras, imagio, PIL, ftplib
</pre>

<pre>
Duration     : May 2020
Last Update  : 05.20.2020
</pre>

<pre>
Domain       : Computer Vision, Machine Learning
Sub-Domain   : Deep Learning, Image Recognition
Techniques   : Deep Convolutional Neural Network, 
Application  : Image Recognition, Image Classification
</pre>

## Works Cited
- [American Thoracic Society](https://www.thoracic.org/professionals/career-development/residents-medical-students/ats-reading-list/adult/pneumonia.php)
- [Stanford CheXNet Model](https://stanfordmlgroup.github.io/projects/chexnet/)
- [Udacity TensorFlow Free Course](https://www.udacity.com/course/intro-to-tensorflow-for-deep-learning--ud187)
- [Keras API](https://keras.io/api/)

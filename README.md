![banner.jpg](https://github.com/a-woodbury/DeepBreath/blob/master/Resources/deepbreathsplash.jpg)

# DeepBreath
<pre>
Domain             : Computer Vision, Machine Learning
Sub-Domain         : Deep Learning, Image Recognition
Techniques         : Deep Convolutional Neural Network, ImageNet, Inception
Application        : Image Recognition, Image Classification, Medical Imaging
</pre>
<pre>
Contributors:
<a href=https://github.com/a-woodbury>Alphonso Woodbury</a>
<a href=https://github.com/viviandng>Vivian Dang</a>
</pre>

![coverphoto.png](https://github.com/viviandng/flatiron-project-4/blob/master/images/xray.png)




### Items in Repository:

- README.md - a summary of the repository content

- [/images](https://github.com/viviandng/flatiron-project-4/tree/master/images) - all images

- [/presentation](https://github.com/viviandng/flatiron-project-4/blob/master/Presentation/Pneumonia%20X-Ray%20Detection.pdf) - PowerPoint and pdf files of the final presentation

  

### Prompt:
According to the [American Thoracic Society](https://www.thoracic.org/patients/patient-resources/resources/top-pneumonia-facts.pdf), Pneumonia is the world’s leading cause of death among children under 5 years of age, killing approximately 2,400 children a day causing it to be the number 1 most common reason for US children to be hospitalized. Although we have adequate treatment for it like our oral and IV antibiotics, IV fluids, oxygen and rehydration therapy, we must be able to detect it and treat it immediately to prevent long term complications and death. </br>

In this project, our goal is to train and build a deep learning model that can classify whether a given patient has pneumonia, given a chest x-ray image.

#### Code
<pre>
GitHub Link      : <a href=https://github.com/viviandng/flatiron-project-4/blob/master/Code/Model_baseline_Dense.ipynb>Model: Baseline, Densely Connected(GitHub) </a>
GitHub Link      : <a href=https://github.com/viviandng/flatiron-project-4/blob/master/Code/Model_CNN.ipynb>Model: CNN (Github) </a>
GitHub Link      : <a href=https://github.com/viviandng/flatiron-project-4/blob/master/Code/Model_DenseNet.ipynb>Model: DenseNet PreTrained (GitHub)</a>
</pre>

#### Dataset
<pre>
Dataset Links    : <a href=https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia>Chest X-Ray Images (Pneumonia) Dataset (Kaggle)</a>
                 : <a href=https://data.mendeley.com/datasets/rscbjbr9sj/2>Chest X-Ray Images (Pneumonia) Dataset (Original Dataset)</a>
</pre>

### Results:

Model | Accuracy | Precision | F1 | **Recall** |
--- | :---: | :---: | :---: | :---: |
Baseline Dense | 0.81 | - | - | n/a
CNN | - | 0.93 | 0.88 - | 0.9
DenseNet | 0.61 | 0.62 | 0.76 | 0.98

### Methodology:

1.	Download the dataset 
2.	Reshape x-rays to  64x64 and create a baseline model with dense layers (fully connected)
3.	Train the data on different models and compare recall scores
    - Densely Connected Neural Network
    - Convolutional Neural Network
    - DenseNet Pretrained
4.	Test the data on the best model (highest recall score)
### Dataset:

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





### Recommendations:

- Incorporate our model to IT softwares (ex: epic) in hospital settings to assist health professionals diagnose pneumonia patients
- Use our model under the supervision of a radiologist to enhance accuracy/recall to improve treatment outcomes which will increase hospitals' ratings and fundings. 

### Next Steps:

- Improve the current model with additional chest x-ray data from adult patients 
- Explore machine learning solutions that detects the cause of pneumonia (viral vs bacterial)


#### Tools / Libraries
<pre>
Languages               : Python
Tools/IDE               : Anaconda
Libraries               : Keras, TensorFlow, Inception, ImageNet
</pre>

#### Dates
<pre>
Duration                : May 2020
Last Update             : 05.08.2020
</pre>

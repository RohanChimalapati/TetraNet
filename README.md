# Project TetraNet Overview

![image](https://user-images.githubusercontent.com/65915193/112793462-f5b15d80-902a-11eb-874b-decbbb800f6d.png)

Project TetraNet is a novel research project used for wildfire mitigation using footage from rapid nanosatellite deployed into space. We created a nanosatellite that utilizes computer vision models, image segmentation U-Net convolutional networks, linear regression artifical neural networks, and mathematical fire spread simulators in order to accurately apply wildfire patterns to a real-world setting, allowing researchers to prevent wildfires from spreading in high-risk regions.

## Nanosatellite Construction

![image](https://user-images.githubusercontent.com/65915193/113235068-11557780-9268-11eb-88a5-1da251bd10b5.png)
![image](https://user-images.githubusercontent.com/65915193/113235206-482b8d80-9268-11eb-9f64-8d097736f1ef.png)

We engineered a nanosatellite to deploy into the Earth's atmosphere from scratch. More information can be found [here](https://drive.google.com/file/d/19KJ8iIdx7iHpYULTgR8Wu4Gu_hYKOD-A/view?usp=sharing).


## Image Segmentation Analysis

Our TetraNet nanosatellite conducts advanced image segmentation analysis to determine the terrain and topology of the land through scanning for dense vegetation on the ground. The images below provide insight into how we created the image segmentation U-Net convolutional neural network.

![image](https://user-images.githubusercontent.com/65915193/113232996-d9e4cc00-9263-11eb-9a9b-24c5d19d305e.png)

The above image was annotated using Apeer to produce the image below. All of our images were obtained through our original footage from our launch to space in 2021 and then annotated similarly using Apeer. 

![image](https://user-images.githubusercontent.com/65915193/113232418-b40af780-9262-11eb-926d-491324db32b6.png)

Afterward, we trained the image segmentation U-Net convolution networks using our annotated images converted to the .tiff format. After applying our trained U-Net to the above image, it produced the image below, showing how our image segmentation model was highly accurate. 


## Predicting Burned Area using Artifical Neural Network

Using the [forest fires data set](http://archive.ics.uci.edu/ml/datasets/Forest+Fires) from the UC Irvine Machine Learning Repository, we created a linear regression artificial neural network trained on this [ForestFires.csv](http://archive.ics.uci.edu/ml/machine-learning-databases/forest-fires/forestfires.csv), which illustrates the hectares of area burned in a forest fire based on input values like temperature, relative humidity, wind, and rain as well as the FFMC, DMC, DC, and ISI indexes.

![image](https://user-images.githubusercontent.com/65915193/113236263-29c69180-926a-11eb-9d14-76c16691f2c6.png)


## Fire Spread Simulation

![image](https://assets.website-files.com/5f45dcafd2144b042ed84cfd/5f45fb0d93892157cded1b01_4168ff14fa8d3045737dbf347ddd91cfcf354931.gif)

## Web Application

We utilized the Python Flask back-end framework to make API calls to Azure's machine learning and cloud services, providing an efficient method of conducting computer vision analysis.

## Utilizing Azure Machine Learning and Cloud Services 

## Practical Applications

Our project is a low-cost alternative to traditional satellites deployed into space that track geographical features and trends. Our satellite can return footage back to Earth to conduct computer vision analysis on certain terrain to analyze its susceptability to wildfires, especially during the threatening summer season, especially in regions like Texas. With the trending temperature increase in global warming, our nanosatellite can provide substantial impact by providing real-time alerts to fire departments and local public safety services to not only mitigate wildfires and save lives but also prevent severe smoke inhalation and save millions of dollars in damage caused by wildfires annually.

## Contributors

Project TetraNet was created by Abhinav Bichal, Sarvesh Sathish, and Pranay Shah for the 2021 Microsoft Azure AI competition.

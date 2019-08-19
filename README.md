# Malaria-detection-using-cell-images
Malaria is a life-threatening disease caused by parasites that are transmitted to people through the bites of infected female Anopheles mosquitoes.
It is preventable and curable.

* In 2017, there were an estimated 219 million cases of malaria in 90 countries.
* Malaria deaths reached 435 000 in 2017.
* The WHO African Region carries a disproportionately high share of the global malaria burden. In 2017, the region was home to 92% of malaria cases and 93% of malaria deaths.

Malaria is caused by Plasmodium parasites. The parasites are spread to people through the bites of infected female Anopheles mosquitoes, called "malaria vectors." There are 5 parasite species that cause malaria in humans, and 2 of these species – P. falciparum and P. vivax – pose the greatest threa
# What is it ?
It is a model built to predict given an image of a cell whether that cell is infected with malaria or not
# Why ?
#### Diagnosis of malaria can be difficult:

* Where malaria is not endemic any more (such as in the United States), health-care providers may not be familiar with the disease.
* Clinicians seeing a malaria patient may forget to consider malaria among the potential diagnoses and not order the needed diagnostic tests. Laboratorians may lack experience with malaria and fail to detect parasites when examining blood smears under the microscope.
* Malaria is an acute febrile illness. In a non-immune individual, symptoms usually appear 10–15 days after the infective mosquito bite. The first symptoms – fever, headache, and chills – may be mild and difficult to recognize as malaria. If not treated within 24 hours, P. falciparum malaria can progress to severe illness, often leading to death.
* Microscopic Diagnosis

Malaria parasites can be identified by examining under the microscope a drop of the patient’s blood, spread out as a “blood smear” on a microscope slide. Prior to examination, the specimen is stained to give the parasites a distinctive appearance. This technique remains the gold standard for laboratory confirmation of malaria. However, it depends on the quality of the reagents, of the microscope, and on the experience of the laboratorian.

#### one can save humans by detecting and deploying Image Cells that contain Malaria or not as it streamlines the process of malaria detection
# Dataset
This Dataset is taken from the official NIH Website: https://ceb.nlm.nih.gov/repositories/malaria-datasets/ 

The Dataset contains two folders and a total of 27558 immages-
  * Parasitized-contains images of cells infected with malaria 
  * Uninfected-contains images of healthy cells
  
![alt text](https://www.kaggleusercontent.com/kf/9195619/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..TKl88IABGLYLN5gt_2L5SQ.fJLhshfX47Pn4rrC4JsJYp6ZDpuK1EO0zVLJC9oGETpW24twxpPZONd83y6R2C3aFPqCMlRcYsff0_aPUKPelqB7SSy_7t6PXmOntn7qLfFgnAvjpCno5bdphfQtVslwzVFVV1UGWv8CboH3lNx0rVHWO6oL9h1T7QQDjltK-zY.3t06mdZHEQYOeS9Q9zpfcg/__results___files/__results___8_0.png)

This dataset is used to train our model which we can later used to predict if the cell is infected or not
# How to run/implement it ?
#### My code is basically the model architecture for the implementations of malaria detecting using CNN
* you can run this code by downloading the dataset provided in this repo and then training the model provided in the malaria ipynb file on that dataset by just executing the malaria ipynb file 
* make sure that the dataset and the malaria ipynb file are saved in the same folder for proper implmentation

#### you can get the output/predicitions on unseen images by using the following code:
```python
img=cv.imread(image_path,0)
img_re=cv.resize(img,(100,100))
model.predict(img_re)
```
#### in order to get predicitions on a photo->
* you need to place image_path with the path address of that image

# References 
* https://www.who.int/news-room/fact-sheets/detail/malaria
* https://www.cdc.gov/malaria/diagnosis_treatment/diagnosis.html


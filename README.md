# Tackling Dengue And Malaria Cases
## Project Details:
**Domain:** Machine Learning           
**Project Name:** Tackling Dengue And Malaria Cases

## Project Description:
**The Problem:** 
Dengue has worsened in Delhi with more than 5,000 cases in 2021, making it the highest number of cases of vector-borne disease recorded in the city in a year since 2015. Dengue is spread to people through the bite of an infected Aedes species mosquito which breeds in damp locations and stagnant water pools.

## Aim:
We will create a dengue information website that shows the predictions of dengue and malaria cases in Delhi in the upcoming months from real time data such as climate such as precipitation, humidity and temperature giving an advanced indicator of when dengue and malaria will emerge and satellite data that will determine the potential dengue hotspots. Through our website people can contact the local government officials in case their area lies in the potential dengue hotspots in order to take necessary actions.


## Data Description:
1. To predict number of dengue cases- We used web scrapping in order to find the number of monthly dengue cases and climate details (precipitation, humidity and  temperature) in Delhi. 
2. To predict number of malaria cases- We used web scrapping in order to find the number of monthly malaria cases and climate details (precipitation, humidity and  temperature) in Delhi. 
3. To obtain sattelite data- We used QGIS to extract Senital 2 sattelite images.


## Model Description:
1. To predict number of dengue cases:
      * We used the dengue data set to train a SVM classifier which includes the following features, year, month, precipitation, humidity, temperature and number of cases per         month. Since this a time series data, so to obtain better results we added a column of previous month's dengue cases. We used different models such as KNN, Random             Forest and SVM. In the end, data trained on SVM gives the best testing result with mean absolute error of 64.
2. To predict number of malaria cases:
      * We used the malaria data set to train a SVM classifier which includes the following features, year, month, precipitation, humidity, temperature and number of cases           per month. Since this a time series data, so to obtain better results we added a column of previous month's malaria cases. We used different models such as KNN,               Random Forest and SVM. In the end, data trained on KNN gives the best testing result with mean absolute error of 16.7.
3. To determine stagnant water:
      * We used QGIS to extract Sentital 2 satellite images. We applied thresholding in order to determine the stagnant water which are potential regions for dengue hotspots. 
 

## Result:
|<img width=50/> ![20](https://user-images.githubusercontent.com/91798475/148248362-fe39e07c-54b1-4ade-a064-2adad609a34f.jpg)| ![19](https://user-images.githubusercontent.com/91798475/148247684-3d10f868-871a-49f5-8831-0b954db552a2.JPG)| ![21](https://user-images.githubusercontent.com/91798475/148248904-673e4264-e4a6-47b5-b1b6-cbb78b6065e7.jpg)| 
| :--:   | :--: | :--: |
| **Dengue Cases** | **Hotspots** | **Malaria Cases** |
|Graph showing comparison of actual dengue cases and predicted dengue cases | Graph showing comparison of actual dengue cases and predicted dengue cases  | Graph showing comparison of actual malaria cases and predicted malaria cases |


## Team Contributors:
Name: Mollika Garg                                                      
Github Link: https://github.com/mollikagarg

Name: Shreya Sharma                 
Github Link: https://github.com/shreya-S51

Name: Koushiki Chakrabarti                     
Github Link: https://github.com/kc2409

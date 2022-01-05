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
1. To predict number of dengue cases- We used web scrapping in order to find the number of monthly dengue and monthly cases and climate details (precipitation, humidity and  temperature) in Delhi. 
2. To obtain sattelite data- We used QGIS to extract Senital 2 sattelite images


## Model Description:
1. To predict number of dengue cases:
      * We used the dengue data set to train a SVM classifier which includes the following features, year, month, precipitation, humidity, temperature and number of cases per         month. Since this a time series data, so to obtain better results we added a column of previous month's dengue cases. We used different models such as KNN, Random             Forest and SVM. In the end, data trained on SVM gives the best testing result with mean absolute error of 64.
2. To predict number of malaria cases:
      * We used the malaria data set to train a SVM classifier which includes the following features, year, month, precipitation, humidity, temperature and number of cases           per month. Since this a time series data, so to obtain better results we added a column of previous month's malaria cases. We used different models such as KNN,               Random Forest and SVM. In the end, data trained on KNN gives the best testing result with mean absolute error of 16.7.
3. To determine stagnant water:
      * We used QGIS to extract Sentital 2 satellite images. We applied thresholding in order to determine the stagnant water which are potential regions for dengue hotspots. 
 

## Result:
| Dengue  | 
| ------------- | 
| * We obtained mean absolute error of 64. |
  * Here is a graph represention of number 
    of actual cases and number of predicted
    cases:                                  
| Content Cell  | 
1. Dengue CASES:                                                     
      * We obtained mean absolute error of 64
      * Here is a graph represention of number 
        of actual cases and number of predicted
        cases:
        ![18](https://user-images.githubusercontent.com/91798475/148244406-6ba289c0-60bf-42a1-a70e-00aed6cbb52e.JPG)


  




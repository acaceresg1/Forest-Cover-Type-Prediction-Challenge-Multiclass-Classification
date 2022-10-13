# Forest_Cover_Type_Prediction_Competition

## Code and Resources Used
**Python Version:** 3.8.14

**Packages:** sci-kit learn, numpy, pandas, matplotlib, seaborn 

## Executive Summary 

Group project for Machine Learning II class at IE university - part of the Masters in Business Analytics and Big Data program.

Predicted forest cover type from four wilderness areas located in the Roosevelt National Forest of northern Colorado. The dataset consists of observations of 30m x 30m patches of land characterized by more than fifty cartographic variables. Using these variables together with a proper machine learning pipeline, it will try to make predictions between the seven different types of trees of each parcel of land included in the test set. First, an exploratory analysis of the training set will be done, followed by a feature engineering process. Once the features are ready to be processed, various models will be trained
and compared in order to find the one which is most suited for our prediction. The best model get an average of 85,3% accuracy (92th percentile Kaggle competition ranking).

## Data Source
Kaggle dataset of 30m by 30m patch of forest land from the Roosvelt National Forest of northern Colorado posted in 2015. Each patch is represented as a row in a training set with over 15K observations and test set with over 565K observations. The analysis requires multi-class classification of the test set where each patch of land should be classified as having one of seven forest cover types:

1. Spruce/Fir
2. Lodgepole Pine
3. Ponderosa Pine
4. Aspen
5. Douglas-fir
6. Krummholz
7. Cottonwood/Willow

## Data Set Features

The training set includes 54 features excluding “id” plus the target variable “Cover Type”. The test set includes only the 54 features.

* 10 numerical: Elevation, Aspect, Slope, Horizontal Distance to Hydrology, Vertical Distance to Hydrology, Horizontal Distance to Roadways, Hillshade 9am, Hillshade Noon, Hillshade 3pm, Horizontal Distance to Fire Points
* Binary (0 absence or 1 presence) for 4 qualitative wilderness areas: Rawah (area with lower mean elevational value), Neota (area with highest mean elevational value), Comanche Peak (area with lower mean elevational value), Cache la Poudre (area with lowest mean elevational value)
* Binary (0 absence or 1 presence) for 40 qualitative soil type designations
* Numerical (integers 1-7) for 7 qualitative cover type designations


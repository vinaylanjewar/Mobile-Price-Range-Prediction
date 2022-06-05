# Mobile-Price-Range-Prediction

![photos mobile](https://user-images.githubusercontent.com/96326032/172070522-a9413a5c-b947-4c30-8bed-e13323165f06.png)


## **Problem statement**:

There are many things we consider before buying a mobile as we used our mobile for various purpose like connecting with our family, playing games, taking a photos to keep our memory. So this such specifications such as RAM, internal memory, Wi-Fi, 3G/4G connectivity etc. plays important role to buy a mobile. To analysis of this important factor from time to time and come up with the best setoff specifications and price ranges so that people will buy the mobile. Hence through the various ML modules we will help the company to estimate the price range of mobiles according to feature so the maximum amount of sell will be possible.

## **Data set Description**:

* Battery_power - Total energy a battery can store in one time measured in mAh
* Blue - Has bluetooth or not
* Clock_speed - speed at which microprocessor executes instructions
*	Dual_sim - Has dual sim support or not
*	Fc - Front Camera mega pixels
*	Four_g - Has 4G or not
*	Int_memory - Internal Memory in Gigabytes
*	M_dep - Mobile Depth in cm
*	Mobile_wt - Weight of mobile phone
*	N_cores - Number of cores of processor
*	Pc - Primary Camera mega pixels
*	Px_height - Pixel Resolution Height
*	Px_width - Pixel Resolution Width
*	Ram - Random Access Memory in Mega Bytes
*	Sc_h - Screen Height of mobile in cm
*	Sc_w - Screen Width of mobile in cm
*	Talk_time - longest time that a single battery charge will last when you are
*	Three_g - Has 3G or not
*	Touch_screen - Has touch screen or not
*	Wifi - Has wifi or not
*	Price_range - This is the target variable with value of 0(low cost), 1(medium cost),2(high cost) and 3(very high cost).

## **Factors Affecting**:

Following are the factors affecting the for price range of mobile :

1.	**RAM** : As the ram size increase the cost of the mobile price also increases.

2.	**Battery Power** : As the Battery Power  increases the price range is also gradually increases.

3.	**Internal Memory** : We observed that there is high price range as the Internal memory size increases.

4.	**Four_G** :  3G /4G mobile phone are categories in high range price.

5.	**Clock speed** : Clock speed has negative correlation with the target variable.

6.	**Wifi** : mobiles which having wifi facility tend to move in high price range mobile group.

## **Steps involved** :

The following steps are involved in the project
1.	**Exploratory Data Analysis** : 
After loading and reading the dataset in notebook, we performed EDA. Comparing target variable which is price range with other independent variables.
This process helped us figuring out various aspects and relationships among the target and the independent variables and also we observed the distribution of variables.
It gave us a better idea that how feature behaves with the target variable.
**Price range vs ram**

![EDA pic](https://user-images.githubusercontent.com/96326032/172070274-fb53fc4a-a060-4626-8a7f-2b774883ad33.png)


2.	**Preprocessing data**  :
Dataset contains a no null values also no duplicate values are found to disturb the accuracy .
Dropping the unwanted columns from the dataset.

3.	**Features selection** :
With the help of exploratory data analysis we analyzed the categorical as well as numerical features in the dataset.And selecting six main feature which are affecting the most.

4.	**Correlation Analysis** :
We plot the heatmap to find  the correlation between both dependent variable and independent variables.

5.	**Train test Split** :
In train test split we take ‘x’ as dependent variables and ‘y’ take as independent variable then train the model.

## **Correlation Analysis**:

![Screenshot 2022-06-06 023018](https://user-images.githubusercontent.com/96326032/172070389-3359cc5e-6b10-45e5-bbc6-c9cda4f70ac4.png)


1.	The highest correlation with respect to the price range is RAM which shows as the RAM increase the Price Range is also increases.
2.	Also as the Battery Power size increase the cost of mobile price range increase.
3.	The dual sim and Four_G facility having positive correlation with the Price range.
4.	There is negative correlation of the mobile weight with respect to the Price Range of mobile as the weight increases the price decreases.
5.	Primary camera and the Front camera has a correlation with price range.

## **Conclusions**:

1.	We build a predictive model, which could help companies to estimate price of mobiles in much effective way.
2.	To predict the cost of various different types of products, same procedure can be performed.
3.	**RAM** in the mobile phones is very important feature for the price range prediction of mobile as the **ram** and **battery power** increases the price range  increases.
4.	According to the user specifications the **camera** plays the important role to attract the customer .
5.	Customer prefers the **longer Battery backup** for long lasting.
6.	**Kneighbors** and **Xgboost** are given best accuracy score 95% test ,93% train and 91% train , 88% test respectively.

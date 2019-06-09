 # Road Accidents Analysis
 
This application is developed to analyse the accidents happened over the last couple of years in the Leeds UK. App is built using Javafx and the accidents data is stored in MySQL database. The application also predicts the number of accidents which may happen in the next 12 months. 


## Analytics presented in the application

This application is an analytics application which tries to extract various facts from the accidents data available and present them in numerous forms including numbers and different forms of visual graphics including Pie chart, Bar chart and Scatter plots.

The overall application targets the casualties and various other related aspects of the accidents such as road conditions, weather conditions, lightening conditions and tries to present measures and facts which can be used to prevent future accidents. Dashboard itself presents the stats on casualties which happened yearly.

## Application dependencies

Application is build using javafx and tagreting jdk 8. It also uses controlsfx for the validation and weka APIs for predictions. Application uses native javafx components for graphical interface including charts and graphs shown.

## Structure of the project

Project structures contains below directories.
1.  Controllers – package to keep controllers
2.  FXML – package to keep fxml files
3.  Images – package to keep images used in the application.
4.  Dao – Utility classes specifically DB interaction and various other utility classes.
5.  Resources – package to keep map components(HTML, JS etc.)

## Core functionalities

Below are the application screens developed as part of the application.
1.  Homepage
2.  User Login
3.  User Signup
4.	Guest Login
5.  Dashboard
6.	Map
7.  Comparison of Accidents
8.  Prediction of Accidents
9.  Scatter Analysis of Accidents
10.  Facts and Preventions
11.  Questions Page for users to submit feedback/questions

### Homepage
Homepage is the very first page which comes up on the start up of the application. Existing users can login to the system using login while new users may signup. Application can be closed using exit butoon.
#
![Homepage](https://github.com/tausy/accident-leeds/blob/master/Road%20Safety%20v1.0/screenshots/Homepage.png)
#
### Login
Using login page, user can login/signup or go back to homepage. One may also choose to continue as a guest.
#
![Loginpage](https://github.com/tausy/accident-leeds/blob/master/Road%20Safety%20v1.0/screenshots/Login.png)
#
### Accidents on Google Map
On map screen, all the accidents are clustered and placed on google map which can be zoom in/out to take a closer look at the accidents happened in an specific area. Moreover, it provides various filters to filter out the specific accidents on the vehicle type, speed, weather conditions, lightening conditions, casulty age etc. A text field with auto completion feature is also provided to search the specific area using postcodes of Leeds UK. 
#
![Map page](https://github.com/tausy/accident-leeds/blob/master/Road%20Safety%20v1.0/screenshots/Map1.png)
#
![Map page](https://github.com/tausy/accident-leeds/blob/master/Road%20Safety%20v1.0/screenshots/Map2.png)
#
### Comparison of accidents
Accidents caused by different vehicles can be compared and visually analysed on yearly basis on this page.
#
![Comparison page](https://github.com/tausy/accident-leeds/blob/master/Road%20Safety%20v1.0/screenshots/Compare.png)
#

### Prediction of Accidents
Number of accidents which may happen in the upcoming months are predicted for next 12 months using Regression and Time lag attributes. Accident data and monthly accident count are considered for predicting the amount of accidents which may occur in next one year. Weka is used for prototyping the model and then the model is used in the javafx application to predict the accidents in future.

Javafx application uses the exported model file from the Weka and use weka java APIs additionally to load the model and train that using the available data and finally predict the number of accidents which may happen in next 12 months.
#
![Predicted Accidents](https://github.com/tausy/accident-leeds/blob/master/Road%20Safety%20v1.0/screenshots/Predict.png)
#

### Scatter Analysis of Accidents
Users can visually analyze the accidents happened over the years due to bad weather/lightening or road surface conditions.
#
![Scatter Accidents](https://github.com/tausy/accident-leeds/blob/master/Road%20Safety%20v1.0/screenshots/ScatterAnalysis.png)
#

### Facts and Preventions
The summarized facts from accidents data are presented here which will be computed from the accidents data present in the database.
#
![Facts Accidents](https://github.com/tausy/accident-leeds/blob/master/Road%20Safety%20v1.0/screenshots/FactsAndPreventions.png)
#


## Class Diagram
![Facts Accidents](https://github.com/tausy/accident-leeds/blob/master/Road%20Safety%20v1.0/diagrams/RoadAccidentsLeeds.png)

## Database Schema
![Facts Accidents](https://github.com/tausy/accident-leeds/blob/master/Road%20Safety%20v1.0/accidentDB.png)


## Dependencies

1.  Java 8
2.  Javafx 8
3.  Mysql 8.5+
4.  Google map apis
5.  Controls fx
6. .Weka

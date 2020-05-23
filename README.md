# Disaster Response Pipeline Project

## Requirements
- Python 3.6
- nltk 3.3.0
- numpy 1.15.2
- pandas 0.23.4
- scikit-learn 0.20.0
- sqlalchemy 1.2.12

## Motivation
In this project, It will provide disaster responses to analyze data from Figure Eight to build a model for an API that classifies disaster messages.

This project will include a web app where an emergency worker can input a new message and get classification results in several categories. The web app will also display visualizations of the data.


## Project Content
- Data
  - process_data.py: reads in the data, cleans and stores it in a SQL database. Basic usage is python process_data.py MESSAGES_DATA CATEGORIES_DATA NAME_FOR_DATABASE
  - disaster_categories.csv and disaster_messages.csv (dataset)
  - DisasterResponse.db: created database from transformed and cleaned data.
- Models
  - train_classifier.py: includes the code necessary to load data, transform it using natural language processing, run a machine learning model using GridSearchCV and train it. Basic usage is python train_classifier.py DATABASE_DIRECTORY SAVENAME_FOR_MODEL
- App
  - run.py: Flask app and the user interface used to predict results and display them.
  - templates: folder containing the html templates

## Example:
> python process_data.py disaster_messages.csv disaster_categories.csv DisasterResponse.db

> python train_classifier.py ../data/DisasterResponse.db classifier.pkl

> python run.py

Live Application URL: https://view6914b2f4-3001.udacity-student-workspaces.com/

## Screenshots
Below are a few screenshots of the web app:


> The main page shows some graphs about training dataset, provided by Figure Eight.
![Alt text](https://github.com/ISMAILHKYILDIZ/Udacity-DataScientist-ND---Project-2---Disaster-Response-Pipeline/blob/master/Web_App_ScreenShot_1.JPG?raw=true "Screenshot1")


> Here is the text box that you can type to test Machine Learning model performance.
![Alt text](https://github.com/ISMAILHKYILDIZ/Udacity-DataScientist-ND---Project-2---Disaster-Response-Pipeline/blob/master/Web_App_ScreenShot_2.JPG?raw=true "Screenshot2")


> After typing example message "there is a fire starting in my house, please help me!" and clicking Classify Message button, you can see the categories which the message predicted by Machine Learning Model highlighted in green.
![Alt text](https://github.com/ISMAILHKYILDIZ/Udacity-DataScientist-ND---Project-2---Disaster-Response-Pipeline/blob/master/Web_App_ScreenShot_3.JPG?raw=true "Screenshot3")


> After typing example message "my leg is broken, call doctor" and clicking Classify Message button, you can see the categories which the message predicted by Machine Learning Model highlighted in green.
![Alt text](https://github.com/ISMAILHKYILDIZ/Udacity-DataScientist-ND---Project-2---Disaster-Response-Pipeline/blob/master/Web_App_ScreenShot_4.JPG?raw=true "Screenshot4")


## Acknowledgements
I wish to thank Figure Eight for dataset, and thank Udacity for advice and review.

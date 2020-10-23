# Introduction

## SQLite-database
SQLite database build using Flask and SQLite-library: [SQLITE](https://www.sqlite.org/index.html) 

## Use case
The database will be used to upload data from various excel files to SQLite database with Python. The first step is to clean the data, then the data is uploaded from pandas dataframe to the SQLite-database. The database is accessed by a Flask application, which will make calls to the database. The Jinja templating engine is used.

## Structure of the Database
There are in total three database tables, which will each include different dataset. Table 1 is used to generate the profiles, table 2 is used to generate the transaction data and table 3 is used to track issues. 

## Flask application
The database will be accessed by the flask-application. The application will visualize data and calculate metrics based for each segment on the dashboard. The overall view illustrates historical developments. The transaction view include forecast and metrics. The issue view allows to take action on cumulated errors and focus future work based on the current metrics.

Web application, includes a dashboard, which purpose is to visualize key metrics under various segmentations.

Forecast view
The forecast view illustrates flagged items vs. non-flagged items based on XGBoost-model. The dataset is generated using Python pandas library.

Dashboard view
Illustrates key metrics based on various segmentation categories. The metrics allow identification of ongoing issues, focus areas and identification well-working business processes.

Database
SQLite database integrates the datasets into single source, which is used by the Flask-based, the front end web application.

Templating
Jinja template-structure segments the Flask application html content into multilayer web application.

# Bokeh-visualization-dashboard
Dashboard with Bokeh-visualizations built on top of Flask web application. This visualization is build with Python and Bokeh-library. The visualizations are rendered on web application based on Flask. The web application templates are build with Jinja.

Bokeh is a python visualization library, which allows visualizations build from pandas dataframes. 

# Final Project Proposal

Zirui Chen & Haoheng tang

## Problem / Question

Currently, the Fire Department has litte ‘situational awareness’ of 
fire risk for a given location when an emergency call comes in. 
Therefore, we are going to help them build a web application that can
gather property infomation, nearest past fire events, violation information,
311 requests, neighborhood information as well as the fire risk given an 
address of a fire event, which can help fire fighter better lead their rescue work.

## The data

We plan to use the API that we built in MUSA practicum. The API can accquire 
property data, code violaiton, cencus data, 311 requests and the fire risk that
we predict all together.

Since the API was built by accquireing data from other API / dataset, we want to include
them here:
1.Philadelphia fire 2015-2020
2.https://cityofphiladelphia.github.io/carto-api-explorer/#public_cases_fc
3.https://cityofphiladelphia.github.io/carto-api-explorer/#violations
4.https://services.arcgis.com/fLeGjb7u4uXqeF9q/arcgis/rest/services/DOR_Parcel/FeatureServer/0/query?outFields=*&where=1%3D1

## Technologies used

(1)leaflet: maps
(2)underscore: data wrangling
(3)JQuery: make html elements interactive
(4)bootstrap
(5)Vector tiles?

## Design spec

#### User experience

- Users: fire fighters who is going to lead rescue work or do daily check for the fire risk
 or residents who want to know the risk of their houses
- Gain: fire fighters can have more information about the property and its surrounding
- Past example？
 

#### Layouts and visual design

![interface](interface.png)

## Anticipated difficulties

Currently our difficulty is: 
(1)How to deal with the large amount of parcel data?
(2)Figuring out how to use the API that we built (we are still trying to deploy it to the cloud) to get data. 

## Missing pieces



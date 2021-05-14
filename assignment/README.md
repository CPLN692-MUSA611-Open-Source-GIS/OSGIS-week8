# Final Project Proposal

Your assignment this week is to write a proposal for your final project.
In proposing your final, try to address each of the following areas.
Please produce at least a paragraph which addresses the topics below

## Problem / Question

Crimes of all kinds happen every day in Philadelphia. 
How many cases occur every day? What kind of cases are more numerous? And in which areas are they located? 
So I hope this final project will provide a simple overview of the crime situation in Philadelphia for users to check.

## The data

The first is a geojson of the Philadelphia police district, as a way to show the crime divisions. 
The second is the crime incidents dataset, which has been updated daily since 2006 and has over 20,000 records in 2021 alone. Therefore, in order to avoid lagging when displaying the map, 
I will use the API to query and display the crimes that occurred in the last 7 days on the map.

## Technologies used


-leaflet to display the map and related elements
-jQuery for dataloading
-underscore as one of libraries to complete basic functions
-API to request data
-boorstrap for a better design and display for the website
-chart to display data

## Design spec

#### User experience

This program is mainly for users who are curious about the crime situation in Philadelphia.

They will get an overview of crime in Philadelphia for the past week from the application, learning the specific number and breakdown of crimes in each district. They can also check the types of cases they want to know about by filtering through mutual attacks.

There are websites designed are actually fancier version of my application.
-https://www.neighborhoodscout.com/pa/philadelphia/crime#data
-http://data.philly.com/philly/crime/?

#### Layouts and visual design

The page will set a header with a logo in the upper left corner and a HELP button（display by modal） in the upper right corner. 
Also a sidebar will be set (which can be shown/hide by the button). 
A legend will be set on the right side to indicate the different colors to distinguish the different case types.

## Anticipated difficulties

Handling data will be more difficult. Although only 7 days of information are currently set up, there are usually nearly 2,000 entries. Also, it is planned to add to let USER self-search the criminal records of different dates, which will also make the processing of DATA more difficult. If it is smoother, we hope to generate the heat intensity of crime density to show the security of different blocks more visually.

## Missing pieces

We've only managed to scratch the surface of the available technologies
by which you could construct an application. What use-cases haven't we covered
that you think would be useful? What technologies not covered seem exciting to
you (you don't necessarily have to fully understand what they're for,
this is a chance for you to get help interpreting a technology's
purpose/usage).


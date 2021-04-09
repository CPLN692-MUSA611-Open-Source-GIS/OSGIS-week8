# Final Project Proposal

Your assignment this week is to write a proposal for your final project.
In proposing your final, try to address each of the following areas.
Please produce at least a paragraph which addresses the topics below

## Problem / Question

Applications are ultimately just tools. What problem or question does
your application attempt to resolve or grapple with? How does your
application speak to this problem/question?

We hope to provide better dining experiences (in Philadelphia) during COVID. After the outbreak of COVID-19, a lot of restaurants were closed at first, then started to offer outdoor dining and partnered up with delivery services. So we hope to create a web application that gathers restaurant information during COVID and COVID cases in the area, so that people can make better decisions on where to eat.

## The data

Geospatial applications are all about working with data. What datasets
would you plan/like to use? If the data you'll be working with isn't
already stored in a way that you can use, how will you be storing your data?
If your data is too large to be conveniently used on the frontend, how will
you work around it? A backend? Vector tiles? Chat with me ASAP if this is
something you need help with!

We are planning on using open data provided by Yelp Fusion APIs (https://www.yelp.com/fusion), Google Place API, and data on COVID-19 cases (https://cityofphiladelphia.github.io/carto-api-explorer/#covid_cases_by_zip). The data from Yelp is in the JSON format and provides information on restaurant location, restaurant type, hours, ratings and reviews. We are thinking about also using Google Place API for more information on the business especially in relation to the changes in service during the pandemic. We are also thinking about using data on COVID-19 cases and their location. We plan to use the API to get the data instead of storing it on a backend. 

Yelp: https://www.yelp.com/fusion
Covid: https://cityofphiladelphia.github.io/carto-api-explorer/#covid_cases_by_zip


## Technologies used

Which technologies covered in class (or discovered on your own!) do you
plan to use? How do you anticipate using each of these technologies?

Review the APIs/online examples of leaflet, turf, jQuery, underscore (or
any library not explicitly covered in class) for functions/uses which
you'd like to explore. Briefly describe how you might use them.

We will be using leaflet for making maps, JQuery for making maps interactive, underscore for fundamental functions to wrangle the data, D3 for data visualization and bootstrap to build the front-end.

## Design spec

#### User experience

At a high level, how do you expect people to use your application?
- Who are the users?
- What do they gain from your application' use?
- Are there any website/application examples in the wild to which you can compare your final?

Users: people who are searching for restaurants during COVID.
Gain: Users will have a better understanding of the restaurant service provided as well as the surrounding area’s cases.
Past example: Our application will be a simplified version of the Yelp App and with more information on COVID cases.

#### Layouts and visual design

So far, we've built all our applications with a side bar for
representing non-map content and navigation. This is not the only
successful design. Extra content could be displayed in a top bar,
through modals, through side bars on both sides, and any combination of
these as well as a number not mentioned. Try to describe your
application's visual layout. Conceptually (no need for extensive CSS
here), what will this design require?

## Anticipated difficulties

Thinking about weaknesses can be useful. What do you anticipate being
most difficult about this project? How will you attempt to cope with
these difficulties? For example, asynchronous behavior (ajax, events)
are hard to use and think about. Global variables are a strategy for
coping with that difficulty by breaking data out of the asynchronous
context.

One difficulty is that we need to figure out how to use the API to get data. Another difficulty is how we can handle the big data set and whether leaflet can handle the data. 

## Missing pieces

We've only managed to scratch the surface of the available technologies
by which you could construct an application. What use-cases haven't we covered
that you think would be useful? What technologies not covered seem exciting to
you (you don't necessarily have to fully understand what they're for,
this is a chance for you to get help interpreting a technology's
purpose/usage).


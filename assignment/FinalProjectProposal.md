# Final Project Proposal: Houston "Greenness" Investigation and Insights on Planning for Community Green Spaces

By Zhijie Zhou

*Your assignment this week is to write a proposal for your final project.*
*In proposing your final, try to address each of the following areas.*
*Please produce at least a paragraph which addresses the topics below*

## Problem / Question

*Applications are ultimately just tools. What problem or question does*
*your application attempt to resolve or grapple with? How does your*
*application speak to this problem/question?*

Debates on development and conservation never ended, as cites themselves never stopped sprawling in the past decades. Rapid expansion and uneven distribution of resources brought about challenges for sustainable and coordinated community growth. How often do you go for a walk in the park or in the woods? This may not be a problem for you if you happen to live close to a park, a community garden, or some other kind of green spaces. However, according to Trust for Public Land's research on urban parks and communities,  more than 1 million people in the United States do not have access to a quality park within a 10-minute walk of home. Besides providing important recreational opportunities for people's wellbeing, green spaces add on the beauty and environmental quality of neighborhoods, and can serve as shelters for urban wildlife, infrastructure for storm water storage, etc.. This project will visualize the "greenness" - including greenery and green spaces, and community profiles for the City of Houston, TX, and provide some insights on planning for community green spaces.

## The data

*Geospatial applications are all about working with data. What datasets*
*would you plan/like to use? If the data you'll be working with isn't*
*already stored in a way that you can use, how will you be storing your data?*
*If your data is too large to be conveniently used on the frontend, how will*
*you work around it? A backend? Vector tiles? Chat with me ASAP if this is*
*something you need help with!*

- American Community Survey - 5 - Year (ACS-5) Data*
- Trust for Public Land (TPL) ParkServe Data*
- Google Street View (GSV) Images
- MapBox API (Directions, etc.)
- NDVI or Landsat/Sentinel Imagery** (to be processed in Google Earth Engine)

Note: 

<small> *ACS-5 data and ParkServe data will be integrated at tract level in a manner similar to the way I did for the midterm project. <br> ** The presentation style of the NDVI data / imagery-based data will depend on whether I choose to create a GEE application or web-interface based on HTML and JS.</small>

## Technologies used

*Which technologies covered in class (or discovered on your own!) do you*
*plan to use? How do you anticipate using each of these technologies?*

*Review the APIs/online examples of leaflet, turf, jQuery, underscore (or*
*any library not explicitly covered in class) for functions/uses which*
*you'd like to explore. Briefly describe how you might use them.*

- MapBox/Leaflet for map display
- Leaflet - draw for user-specified point/polygons on map area to display parks or other features and metrics per user's interest.
- jQuery for data request - also enable changeable content display with clicks (on each feature/region) 
- Templates/Bootstrap for web interface design
- MapBox API for route-finding, etc.
- GSV processing in python (inspired by https://github.com/larkinandy/GSV_NDVI_Comparison, though that project was based on C++)

## Design spec

#### User experience

*At a high level, how do you expect people to use your application?*
- *Who are the users?*
  - Planners, or whoever interested in the integrated planning process
- *What do they gain from your application' use?*
  - More knowledge about community access to green spaces and the spatial distribution of green spaces in Houston.
  - Potential room for decision metrics for planning.
- *Are there any website/application examples in the wild to which you can compare your final?*
  - TPL has a ParkServe application for each American city in which they provide suggestions for park planning.

#### Layouts and visual design

*So far, we've built all our applications with a side bar for*
*representing non-map content and navigation. This is not the only*
*successful design. Extra content could be displayed in a top bar,*
*through modals, through side bars on both sides, and any combination of*
*these as well as a number not mentioned. Try to describe your*
*application's visual layout. Conceptually (no need for extensive CSS*
*here), what will this design require?*

- Map with floating windows?
- GEE app with drawing tools?
- Allow user to zoomin/out to different display contents with clickable features

## Anticipated difficulties

*Thinking about weaknesses can be useful. What do you anticipate being*
*most difficult about this project? How will you attempt to cope with*
*these difficulties? For example, asynchronous behavior (ajax, events)*
*are hard to use and think about. Global variables are a strategy for*
*coping with that difficulty by breaking data out of the asynchronous*
*context.*

- data storage: github repo? AWS cloud?
- more user-interactions with drawing tools

## Missing pieces

*We've only managed to scratch the surface of the available technologies*
*by which you could construct an application. What use-cases haven't we covered*
*that you think would be useful? What technologies not covered seem exciting to*
*you (you don't necessarily have to fully understand what they're for,*
*this is a chance for you to get help interpreting a technology's*
*purpose/usage).*

- Calling for processing other datasets when user clicks on one particular feature of the first layer displayed?
- smooth transition among displays


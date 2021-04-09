# Final Project Proposal: Impacts of Transit Oriented Developments (TOD)
 
Your assignment this week is to write a proposal for your final project.
In proposing your final, try to address each of the following areas.
Please produce at least a paragraph which addresses the topics below
 
## Problem / Question
 
Applications are ultimately just tools. What problem or question does
your application attempts to resolve or grapple with? How does your
application speaks to this problem/question?
 
This project will attempt to illustrate impact of Transit Oriented Development (TOD) in San Francisco (SF) on various components, including property values and social equity issues. TOD has been promoted in the last decades to encourage transit ridership, but for various cases it has been a pusher of gentrification. To examine whether this is an empirical case across the city (cross-sectional) and across years (longitudinal), and to identify the distribution of TOD and its impacts between TOD and non-TOD, our map application will visually present the information through maps and charts. Our application may also serve as a tool for users to compare information between individual TOD properties. Xinyi and I have agreed to work on this as a group.
 
## The data
 
Geospatial applications are all about working with data. What datasets
would you plan/like to use? If the data you'll be working with isn't
already stored in a way that you can use, how will you be storing your data?
If your data is too large to be conveniently used on the frontend, how will
you work around it? A backend? Vector tiles? Chat with me ASAP if this is
something you need help with!
 
 
Property value data: https://data.sfgov.org/Housing-and-Buildings/Assessor-Historical-Secured-Property-Tax-Rolls/wv5m-vpq2
Transit station data: https://github.com/gxzhao1/SF-TOD-DEV \ https://github.com/gxzhao1/SF-TOD-DEV 
(+ Census Data)
 
We will process the data in R to determine whether the property is within a TOD buffer (~0.5 mile buffer). The dataset is large so we will use RSocrata package \ SODA API to access the data. Then we will store the data in GeoJSON format to read into JS. If the file is too big, we will filter the data by year (ex. 2015-2019). These are our main concerns and we would appreciate specific feedback to smoothen our workflow.
 
## Technologies used
 
Which technologies covered in class (or discovered on your own!) do you
plan to use? How do you anticipate using each of these technologies?
 
Review the APIs/online examples of leaflet, turf, jQuery, underscore (or
any library not explicitly covered in class) for functions/uses which
you'd like to explore. Briefly describe how you might use them.
 
We plan to work with many of the technologies covered in class, including Leaflet, jQuery, underscore, and turf (for buffer visualization). We plan to use Leaflet for basic visualization, displaying properties as points and transit stations as points (with a line signifying the track). We plan to use jQuery and underscore for basic data manipulation, including filtering, grouping, etc. We also want to use turf to enable more advanced spatial manipulation such as adding a buffer (circle) to the stations, or calculating the distance from transit stations to property points. Inspired by the Philly building energy benchemarking website, we would also want to advance our skills with charts to illustrate the comparisons.
*Example for chart js: https://appstack-react.bootlab.io/charts/chartjs 
 
## Design spec
 
#### User experience
 
At a high level, how do you expect people to use your application?
- Who are the users? Developers; planners; homeowners/homebuyers
- What do they gain from your application' use? Help them examine the development trend and opportunities for TOD in SF. If we have time, we can also look into TOD and equity to see if TOD aggravates living segregation between different races and income groups.
- Are there any website/application examples in the wild to which you can compare your final?
The Philly building energy benchmarking for aesthetics; 
A illustration of TOD and property data: http://growchicago.metroplanning.org/?utm_source=%2fgrowchicago&utm_medium=web&utm_campaign=redirect  
A illustration of TOD map: https://mrutzen1.carto.com/viz/acf12362-4695-11e5-b932-0e0c41326911/embed_map 
An example website on TOD: https://etod.cnt.org/#tool
 
 
#### Layouts and visual design
 
So far, we've built all our applications with a side bar for
representing non-map content and navigation. This is not the only
successful design. Extra content could be displayed in a top bar,
through modals, through side bars on both sides, and any combination of
these as well as a number not mentioned. Try to describe your
application's visual layout. Conceptually (no need for extensive CSS
here), what will this design require?
 
A footer to the bottom of the viewport with a fixed top navbar: https://getbootstrap.com/docs/5.0/examples/sticky-footer-navbar/
A cover page or modal: https://getbootstrap.com/docs/5.0/examples/cover/
    Two option: 1. interactive map; (2. story map to guide navigations to tell a story (like midterm))
        (For the map: click on the marker can enable comparison between that property and the overall distribution)
Header or floating/collapseable "header/sidebar": https://themes.getbootstrap.com/preview/?theme_id=35393
    with input boxes for 1: insert address for zooming in; 2. type for property type; 3. value by types of property value; 

## Anticipated difficulties
 
Thinking about weaknesses can be useful. What do you anticipate being
most difficult about this project? How will you attempt to cope with
these difficulties? For example, asynchronous behavior (ajax, events)
are hard to use and think about. Global variables are a strategy for
coping with that difficulty by breaking data out of the asynchronous
context.

As of for now, we are not experienced with building charts, so we don't know how difficult that will be. We are also not certain about how to pre-process the data before loading into javascript. We are afraid that just data manipulation will take a lot of time given the size of the dataset.
 
## Missing pieces
 
We've only managed to scratch the surface of the available technologies
by which you could construct an application. What use-cases haven't we covered
that you think would be useful? What technologies not covered seem exciting to
you (you don't necessarily have to fully understand what they're for,
this is a chance for you to get help interpreting a technology's
purpose/usage).

Building slidebar would be cool.
Maybe also a slider on the map that can alternative between different maps.
These are not relevant to our project, but a user system (log in, storing information) would be cool.
Incorporating google maps API would also be helpful since a lot of users are used to the google interface.

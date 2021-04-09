# Final Project Proposal

Your assignment this week is to write a proposal for your final project.
In proposing your final, try to address each of the following areas.
Please produce at least a paragraph which addresses the topics below

## Problem / Question

Applications are ultimately just tools. What problem or question does
your application attempt to resolve or grapple with? How does your
application speak to this problem/question?

* - Provide developers with a quick tool to view and filter current multi-family
comps throughout NYC *
* - Users will be able to view selected properties both on the map and in a list
form to the left of the page*

## The data

Geospatial applications are all about working with data. What datasets
would you plan/like to use? If the data you'll be working with isn't
already stored in a way that you can use, how will you be storing your data?
If your data is too large to be conveniently used on the frontend, how will
you work around it? A backend? Vector tiles? Chat with me ASAP if this is
something you need help with!

*Data points will need to be collected manually from reading news articles on new construction
and taking buildings worth noting from Streeteasy.com. Data will first be entered into Google Map
to form a KML file before imported into js file.*

## Technologies used

Which technologies covered in class (or discovered on your own!) do you
plan to use? How do you anticipate using each of these technologies?

Review the APIs/online examples of leaflet, turf, jQuery, underscore (or
any library not explicitly covered in class) for functions/uses which
you'd like to explore. Briefly describe how you might use them.

* - leaflet-kml to load and display the KML file *
* - leaflet cifrcle marker to pinpoint properties on the map *
* - bootstrap for sidebar design *
* - jquery to handle user input and filter functions*

## Design spec

#### User experience

At a high level, how do you expect people to use your application?
- Who are the users? *developers*
- What do they gain from your application' use? *quick glance and easy selection of comps to their like*
- Are there any website/application examples in the wild to which you can compare your final?
*Perhaps Zillow?*

#### Layouts and visual design

So far, we've built all our applications with a side bar for
representing non-map content and navigation. This is not the only
successful design. Extra content could be displayed in a top bar,
through modals, through side bars on both sides, and any combination of
these as well as a number not mentioned. Try to describe your
application's visual layout. Conceptually (no need for extensive CSS
here), what will this design require?
* - a list of selected properties on the sidebar*
* - a few search and filter bars on the side bar*
* - map to the right*

## Anticipated difficulties

Thinking about weaknesses can be useful. What do you anticipate being
most difficult about this project? How will you attempt to cope with
these difficulties? For example, asynchronous behavior (ajax, events)
are hard to use and think about. Global variables are a strategy for
coping with that difficulty by breaking data out of the asynchronous
context.

## Missing pieces

We've only managed to scratch the surface of the available technologies
by which you could construct an application. What use-cases haven't we covered
that you think would be useful? What technologies not covered seem exciting to
you (you don't necessarily have to fully understand what they're for,
this is a chance for you to get help interpreting a technology's
purpose/usage).
* It'd be a lot easier if we could just mine data from Streeteasy instead of 
manually input them into a KML file*

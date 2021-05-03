# Final Project Proposal

Your assignment this week is to write a proposal for your final project.
In proposing your final, try to address each of the following areas.
Please produce at least a paragraph which addresses the topics below

## Problem / Question

Applications are ultimately just tools. What problem or question does
your application attempt to resolve or grapple with? How does your
application speak to this problem/question?

This application aims at showing the usage of bikeshare stations in Philadelphia.
This helps the city measure the needs for bikeshare services and also the
bikeshare company when deciding where to locate their stations to make the most
profits. The bikeshare stations will be presented by circles on the map and bigger
the circle, the more popular is this station. Moreover, we can also filter
these stations by passholder types and day of the week, so we can have a clearer
understanding of how the demand varies by pass type and day of the week (by hour?). By clicking/
moving the mouse over each station, we can see a pop up with chart showing
the variation of demand by day of the week for each station.

## The data

Geospatial applications are all about working with data. What datasets
would you plan/like to use? If the data you'll be working with isn't
already stored in a way that you can use, how will you be storing your data?
If your data is too large to be conveniently used on the frontend, how will
you work around it? A backend? Vector tiles? Chat with me ASAP if this is
something you need help with!

The data will be the Indego bikeshare data for week 44 in 2018.

## Technologies used

Which technologies covered in class (or discovered on your own!) do you
plan to use? How do you anticipate using each of these technologies?

Review the APIs/online examples of leaflet, turf, jQuery, underscore (or
any library not explicitly covered in class) for functions/uses which
you'd like to explore. Briefly describe how you might use them.

## Design spec

#### User experience

At a high level, how do you expect people to use your application?
- Who are the users?
- What do they gain from your application' use?
- Are there any website/application examples in the wild to which you can compare your final?

The users can be the city, bikeshare companies as well as the general public
who are interested in this information.

https://www.rideindego.com/stations/

#### Layouts and visual design

So far, we've built all our applications with a side bar for
representing non-map content and navigation. This is not the only
successful design. Extra content could be displayed in a top bar,
through modals, through side bars on both sides, and any combination of
these as well as a number not mentioned. Try to describe your
application's visual layout. Conceptually (no need for extensive CSS
here), what will this design require?

https://www.figma.com/file/n8BGQTBcWGcYTZwWKhiwWz/MUSA-611-FINAL-PROJECT?node-id=0%3A1

## Anticipated difficulties

Thinking about weaknesses can be useful. What do you anticipate being
most difficult about this project? How will you attempt to cope with
these difficulties? For example, asynchronous behavior (ajax, events)
are hard to use and think about. Global variables are a strategy for
coping with that difficulty by breaking data out of the asynchronous
context.

1. arrange this bike records and group them by stations.
2. the switch of day of week chart and hour of the day chart.

## Missing pieces

We've only managed to scratch the surface of the available technologies
by which you could construct an application. What use-cases haven't we covered
that you think would be useful? What technologies not covered seem exciting to
you (you don't necessarily have to fully understand what they're for,
this is a chance for you to get help interpreting a technology's
purpose/usage).

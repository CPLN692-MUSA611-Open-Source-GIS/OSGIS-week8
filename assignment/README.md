# Final Project Proposal: NTD Ridership Dashboard
Ben Dodson

## Problem / Question

The US Department of Transportation's Federal Transit Adminstration maintains data on the nation's public transit operations through the National Transit Database (NTD). Versions of the NTD are published on a annual and monthly basis. Ridership is one metric that is published on a monthly basis. The FTA does not maintain an API for this data so it requires a manual process to download, format, and visualize the data. My solution is to create a dashboard on the ridership data to make this dataset more accessible to all. With large swings in ridership during the past few months' period of decline and growth, this data is extremely valuable to transportation planners. The NTD enables comparisons across services to see if peer agencies or services within an agency are experiencing the same ridership trends. I personally use this data on a regular basis to provide estimates of commuter rail ridership in the Northeast. The dashboard will enable the ability to view ridership statistics for all agencies, by month, mode, and whether the service is directly operated or contracted out and comparisons across these categories.

## The data

The dataset is relatively small (3MB in a csv format) and additional variables from the ACS can be included at the metro-area (UZA) level as the data is already tagged with this. This would allow for ridership to be normalized across variables like population and service area.

## Technologies used

I plan to base this off a Bootstrap dashboard example and build out custom graphs for these variables. Some jquery and/or underscore functions will be necessary to filter and compare the data. The dataset itself can be kept within the repo. Leaflet can be used for various map visuals including chloropleth and bubble maps to visualize ridership at the metro-area level.

## Design spec

#### User experience

This dashboard would be very helpful to transportation planners and policy makers who are monitoring the trends in public transit ridership around the country. Higher than average ridership could be an indictator of recovery in an area and may reflect other externalities like local or modal hesistancy towards returning to transit and the return of office commuters. The dashboard will be setup in a way, through the language used, to be publically-digestable without any technical backgorund in transportation planning. This would allow people outside of the immediate industry such as real estate developers and economic development analysts to understand how public transit ridership can be an indicator of economic activity.

#### Layouts and visual design

This dashboard will involve a vertical, top-level navigation bar allowing the user to thumb through the different cuts of the data. Ideally, the view of the data on each dashboard page will grow more focused as the user moves down the list of pages. 

- Landing Page (Orienting the user to the site and how to use)
- National View
    - Map of US with bubbles representing transit ridership for each metro area
    - Line graph showing total transit ridership over last 3, 5, and 10 years
    - Cards or pie graph showing totals by mode, largest transit operator
- Modal View
    - Public transit mode dropdown
    - Graph showing total ridership for that mode
    - Breakdown of directly operated versus contracted operations
    - Map of ridership
    - Graph displaying how this mode compares to others
- Metro Area View
    - Metro area dropdown
    - Modal profile of the metro area
    - Operations breakdown of the metro area
    - Chart of ridership
    - Metro area basic details from ACS (size, pop, income, primary mode to work breakdown)
    - Graph displaying how this metro area compares to others
- Operator View
    - Dropdown of top 30 largest operators
    - Breakdown of ridership on that system
    - Breakdown of operations (direct or contracted)
    - Chart showing ridership by mode
    - Graph displaying how this operator compares to the other top 30

## Anticipated difficulties

I will have to explore the best solutions for the graphing parts of this dashboard. I am familiar with the basic graphs (bar, line, pie) but there may be some interactive infographics that could prove a better visualization of this data and better take advantage of the fact it is an interactive platform.

## Missing pieces

Overview of graphing packages would be helpful!
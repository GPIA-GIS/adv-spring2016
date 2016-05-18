---
layout: project-page
title: "Resources to Facilitate Greyston's Open Hiring Initiative"
linkname: resources-to-facilitate-greyston-s-open-hiring-initiative
author: "Kobi Loehr"
tagline: "Website with maps Greyston can use to help both themselves and other businesses expand Open Hiring practices"
location:
    - place: Yonkers, NY
project-link:
    - href: https://loehk550.github.io/2016/AdvancedGIS/home104.html
tags:
    - tag: #workforcedevelopment
    - tag:  #poverty
    - tag:  #openhiring
    - tag:  #alternativehiring
    - tag:  #communityorganizations
thumbnail-path: img/resources-to-facilitate-greyston-s-open-hiring-initiative/fXHBf3Q.jpg
img-folder: ../../img/resources-to-facilitate-greyston-s-open-hiring-initiative/
timestamp: 5/16/2016 18:13:09
---
HOME
![]({{ page.img-folder }}UjjZecA.jpg)
The homepage of the website includes an introduction to the purpose of the site and some brief descriptions of where each button links to and why.  Greyston has been utilizing Open Hiring for over 30 years.  Open Hiring is a process in which Greyston hires any person who is willing to show up and work hard - no questions asked.  Open Hiring requires that employers make no inquiries regarding the educational, work, or criminal history of their employees.  This model works for Greyston, in part, because they provide assistance to Open Hire employees for childcare needs, substance abuse or mental health counseling, and affordable housing applications.  Greyston is seeking to influence other employers in Yonkers to adopt the Open Hiring model.  Greyston knows that employers will need to be convinced to utilize the model (see "Yonkers") and will need help locating resources within the community that Open Hired employees often need (see "Community Resources").  Greyston is also looking to identify other businesses that may be interested in utilizing Open Hiring (see "Open Hiring Resources").  This website addresses these needs. The buttons at the top of each page link to other pages hosting maps.

COMMUNITY RESOURCES
<iframe width="100%" height="520" frameborder="0" src="https://greymaps104.cartodb.com/viz/2cecd3fa-0e40-11e6-bed1-0e98b61680bf/embed_map" allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>
This page hosts a map with Various Community Resources that could be utilized by HR departments at other businesses that utilize Open Hiring in the future.  The map has info windows that provide necessary details for each organization.  There is also a drop-down menu that sorts the organizations by category (see below for an example).
![]({{ page.img-folder }}axhDEeh.jpg)

OPEN HIRING RESOURCES
<iframe width="100%" height="520" frameborder="0" src="https://greymaps104.cartodb.com/viz/f25ab4a4-1250-11e6-9feb-0ef24382571b/embed_map" allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>
Similar to the Community Resources page, the Open Hiring Resources page hosts a map that shows identified options for businesses that may consider Open Hiring practices.  Research suggested that businesses that had worked with Greyston in other capacities in the past, were family or minority owned, or promoted their strong ties to the community would be the best possible options for Open Hiring outreach.  Info windows provide information about these businesses as well as the status of Greyston's outreach to the businesses (see "Instructions to Update Map Data").  There is also a similar drop down menu on this page that allows Greyston to search by job type, with the job types corresponding to their existing workforce development programs.

YONKERS
This page hosts for maps that highlight some economic and demographic disparities between Southwest Yonkers (the most impoverished area of Yonkers) against the rest of the community.  This page is meant to serve as a tool to highlight why Open Hiring is important (poverty alleviation) and the conditions that many Open Hired employees face in their neighborhoods.  The page highlights main conclusions from each map and provides a brief description of each map. The four maps are imbedded below.  The maps include info windows that provide specific measures for each census tract, however the choropleth maps are designed to visually show the differences using the legends.
Income:
<iframe width="100%" height="520" frameborder="0" src="https://greymaps104.cartodb.com/viz/64a7e426-1b86-11e6-aa33-0e3a376473ab/embed_map" allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>
Housing Prices:
<iframe width="100%" height="520" frameborder="0" src="https://greymaps104.cartodb.com/viz/c48b15d4-1b8b-11e6-b7df-0e674067d321/embed_map" allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>
Non-White Residents:
<iframe width="100%" height="520" frameborder="0" src="https://greymaps104.cartodb.com/viz/0313f6c6-1b88-11e6-8185-0e31c9be1b51/embed_map" allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>
Population Density:
<iframe width="100%" height="520" frameborder="0" src="https://greymaps104.cartodb.com/viz/a343165a-1b8c-11e6-8473-0e787de82d45/embed_map" allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>

INSTRUCTIONS TO UPDATE MAP DATA
This button appears at the bottom of the Community Resources and Open Hiring Resources pages and provides Greyston with instructions to update map data in CartoDB.  This allows Greyston to track their outreach to businesses using the CartoDB data or to add new points as necessary.
![]({{ page.img-folder }}ByiPnxR.jpg)

Methodology:  The Greyston Foundation was my client for the Urban policy Lab course at the New School.  They are seeking ways to influence other businesses in Yonkers to utilize Open Hiring.  As a benefit corporation that began specifically to hire hard-to-employ individuals, Greyston has resources and goals that make them unique within the Yonkers business community.  After identifying the need for the resources created for this project, I began looking for data to complete the maps.  Community Resources data was created by Google searches for different types of resources, confirming the validity of the resources and information found (often via phone calls), and geocoding the addresses found (primarily using Google maps).  A similar process was utilized for the Open Hiring Resources map, however more research was done for each point, including identifying the necessary characteristics for each business that would make them possible Open Hiring candidates.  The four maps on the Yonkers page were created by accessing the Westchester County census tract shapefiles from the US Census Bureau, cutting out only the Yonkers census tracts, and inputing the necessary economic and demographic data for each (avg. income, avg. housing prices, % non-white residents, and population density).  The polygon for Southwest Yonkers was created in CartoDB (by hand) after comparing multiple images that identified the area.  I was not able to locate a shapefile or a formal definition of Southwest Yonkers, but the area outlined in each map seems to correspond closely to a few images that I was able to find that define the area.  I created the base map used for each map in MapBox and all maps were created in CartoDB.

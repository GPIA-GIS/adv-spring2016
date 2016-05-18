---
layout: project-page
title: "Medicare Accountable Care Organizations & Poverty Rates"
linkname: medicare-accountable-care-organizations-poverty-rates
author: "Clare Churchouse"
tagline: "Investigation of Medicare ACOs locations in relation to counties with higher poverty rates and greater health care vulnerability."
location:
    - place: Contiguous USA
project-link:
    - href: http://churc.github.io/house-ACO/
tags:
    - tag: health care
    - tag:  vulnerability
    - tag:  accountable care organizations
    - tag:  medicare
    - tag:  poverty
thumbnail-path: img/medicare-accountable-care-organizations-poverty-rates/rJD1rfJ.png
img-folder: ../../img/medicare-accountable-care-organizations-poverty-rates/
timestamp: 5/16/2016 23:58:54
---
In 2011, The Centers for Medicare and Medicaid Services (CMS) announced the Accountable Care Organization (ACO) model enabling health care systems to coordinate care together in shared savings programs. By February 2016, an estimated 838 ACOs were operating in the United States, of which 433 were Medicare ACOs. Each ACO makes a 3-year commitment, bringing provider participants (doctors, hospitals and other health care providers) together to form networks to coordinate patient care. Data on this relatively new health care model is being collected and assessed. These national maps aim to add information to the current analyses of Medicare Shared Savings Program Accountable Care Organizations by visualizing locations in comparison to selected health care vulnerability indicators, with a focus on areas of higher poverty.

Using CMS Medicare ACO data at data.cms.gov, I geocoded the earlier years using Batch Geocode and mapped 2014, 2015 and 2016 locations.

![]({{ page.img-folder }}MrcV07i.png)

Due to data limitations, Medicare data only is used here, a little over half of the total ACO dataset. The Medicare provider information details 14,817 participants in February 2016. I did some preliminary maps to visualize by year, and one to show the relative size of the organizations by number of providers.

<iframe width="100%" height="520" frameborder="0" src="https://thenewschool.cartodb.com/u/churc186/viz/b5b1f48e-14dc-11e6-b753-0e31c9be1b51/embed_map" allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>

I decided to use ACO locations rather than the provider participant addresses (many of the providers list their locations as their organization address; therefore, I choose the ACO dataset as the most accurate to work from). I mapped these locations in relation to population, using ACS Tiger Urban Area U.S. 2014 shapefiles. Spatially joining the datasets showed that 87% of organization locations are in urban areas or urban clusters.

<iframe width="100%" height="520" frameborder="0" src="https://thenewschool.cartodb.com/u/churc186/viz/dc30b2b6-149c-11e6-90aa-0e5db1731f59/embed_map" allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>

In addition to mapping at the county level, I also mapped the locations to Dartmouth Atlas of Health Care’s Hospital Referral Regions to look for comparisons. I selected, though, to go with county data from the US Census American Community Survey 2014, 5 Year Survey in order to access detailed health care indicators. 
By spatially joining the ACS tables and CMS Medicare ACOs, I made 6 maps to compare patterns of high vulnerability for rates per county for poverty, high school graduation, disability, 65 years and older, Black or African American alone, and Hispanic or Latino of any race. Choropleth, three equal interval, were used throughout and dropdown menus were made to select by percent. 2016 Medicare ACO locations are overlaid on top. Similar patterns across indicators were emphasized by grouping in pairs (e.g. poverty and high school graduate rates). Below is one map of 65 years or older county rates, 2014 ACS 5 Year: S0101. Medicare is a program for those who are 65 and older (as well as for certain younger people with disabilities, and people with End-Stage Renal Disease) - however, with the exception of Florida, this map shows the location of many ACOs are in counties with lower older age population rates.

<iframe width="100%" height="520" frameborder="0" src="https://thenewschool.cartodb.com/u/churc186/viz/bdf8c93c-0f1a-11e6-81c0-0ecd1babdde5/embed_map" allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>

I then turned to focus on poverty, a known indicator of worse health outcomes, to assess poverty county rates in relation to ACO locations. Mapping information on Medicare ACOs onto a detailed basemap, I included dropdown selectors for track, agreement type, and number of provider participants per organization, and infowindows with location information, start date and web link. The 433 Medicare ACOs are located in 234 counties. Using PostGIS, a twenty-mile buffer was created around each location as an estimated distance for patients to travel for health care. The dataset was joined in QGIS with the ACS S1701: percent below poverty level. Poverty rates divide by equal intervals into three groups: 
•	Low: 1% - 18.2% 
•	Mid: 18.2% - 35.4% 
•	High: 35.4% - 52.6% 

3,142 counties were used for this analysis - the poverty dataset omits State FIPS 60: American Samoa, 66: Guam, 69: Northern Mariana Islands, 72: Puerto Rico, and 78: Virgin Islands of the U.S.  
Mid and high-poverty counties were selected, and using PostGIS, I removed those which intersected with the Medicare ACO buffers. The resulting dataset contained counties with poverty rates over 18.2% that were not within 20 miles of a Medicare ACO.

<iframe width="100%" height="520" frameborder="0" src="https://thenewschool.cartodb.com/u/churc186/viz/3441dc88-f84f-11e5-b332-0e5db1731f59/embed_map" allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>

As compared to the visualization of mid and high poverty rates across the country with no counties removed adjacent to Medicare ACO locations - shown in light orange compared to the blue outside the buffer areas.
Map analysis revealed that 1,138 counties (36.22%) out of 3,142 have poverty rates greater than 18.2%. Of those:
•	199 (17.49%) mid and high poverty level counties have a Medicare ACOs within 20 miles.
•	939 (82.51%) mid and high poverty counties do not have a Medicare ACO within 20 miles.

![]({{ page.img-folder }}r20bVNw.png)

Of the 939 counties without a Medicare ACO within 20 miles: 
•	43 (4.58%) of these counties have a poverty rate over 35.4% 
•	896 (95.42%) of these counties have a poverty rate between 18.2% and 35.4%

These maps do visualize high vulnerability levels in counties that are not close to a Medicare ACO location. However, it must be noted that the health care organizations are mainly in urban areas; therefore, mapping location only, without controlling for population, is a limitation. Another issue is that there are not many Medicare ACOs compared to 3,142 counties, and the 433 organizations are only in 234 counties, thus comparing at the state level in addition may be useful. The size variation from one to 328 providers, and mapping only Medicare, rather than all types of Accountable Care Organizations, also restrict the conclusions that can be drawn.

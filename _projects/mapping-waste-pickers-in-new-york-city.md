---
layout: project-page
title: "MAPPING WASTE PICKERS IN NEW YORK CITY"
linkname: mapping-waste-pickers-in-new-york-city
author: "Silvia Xavier"
tagline: "Canners contribute to recycling, but they often go unnoticed and unheard. Here we map their collection routes, their practices and stories."
location:
    - place: New York, NY, USA
project-link:
    - href: http://silviaxavier.github.io/canners.html
tags:
    - tag: Recycling, waste pickers, canners, social justic
thumbnail-path: img/mapping-waste-pickers-in-new-york-city/Wg9O3ty.jpg
img-folder: ../../img/mapping-waste-pickers-in-new-york-city/
timestamp: 5/16/2016 22:32:28
---
In New York City waste pickers walk the streets, usually carrying a cart, to collect discarded beverage containers that can be exchanged for 5¢ each. This process of exchanging discarded containers for money - the 5¢ is actually a deposit initiated when the beverage is bought - is determined by the New York State Returnable Container Act, the Bottle Bill. This is an Extended Producer Responsibility Law that was created in the early 1980s to incentivize recycling. Nowadays, individuals in a economically and socially vulnerable situation take advantage of this legal framework to earn a living or complement their income. Commonly known as canners, these individuals contribute to retrieve recyclables in the city. Moreover, ‘canning’ is also a way to have a economically productive activity.

![]({{ page.img-folder }}bRNF3G1.jpg)

Despite the social and environmental benefits of canning, city authorities oppose the activity. One of the arguments is that they don’t have data for this collection, so the materials retrieved by canners are not accounted for in the city’s diversion rate. This project is an effort to gather data for the canners’ system. Not necessarily quantitative data that can be used in the city’s recycling rate, but a mix of quantitative and qualitative data that documents the spatial and material dynamics of canning and record the individuals’ voices, practices and stories. The goal is to quantify and humanize the waste collection activity. 

![]({{ page.img-folder }}2Ce23t3.jpg) 

For this purpose, I had to carry out field research for data collection, because this dataset was non-existent. I got in touch with canners, explained the project, and asked if I could join them for a day of work. When walking with the canner, I used a mobile phone with a GPS app to track the route. The data exported from the GPS app contained points with recorded location and time, which was perfect for my purpose.  

![]({{ page.img-folder }}s2YI9Rr.jpg)

Throughout the way, I took notes of the quantities and types of materials that were being collected. I recorded the location, so I could then relate it to the GPS data, and I took note of additional characteristics for each location - collecting from street bin, from bag placed at the curbside, from the floor, etc. In addition, I took notes of other interesting events, such as meeting a friend, having an interesting conversation, or picking up the cart from where it was parked. All these events were part of my field notes. 

![]({{ page.img-folder }}hbq0ahE.jpg)

Connecting the field notes to the GPS data was challenging, I had to organize and translate the information I had on paper to make it fit in columns and rows in a way that made sense to be displayed. Editing the dataset in QGIS and inputting the information that was recorded on paper demanded time and attention.

![]({{ page.img-folder }}HBwMks7.jpg)

Finally, having the dataset ready, I used the torque feature in CartoDB to animate the canners’ paths, and I edited and styled the features in the dataset to include audio, pictures, and to show the locations and the types of collection. 

<iframe width="100%" height="520" frameborder="0" src="https://xavis637.cartodb.com/viz/5a346274-e4ab-11e5-9257-0e787de82d45/embed_map" allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>

I compiled the three datasets that I have in one website. In this page, I pulled the data from CartoDB to calculate the amount of materials collected in the canning day. 

http://silviaxavier.github.io/canners.html
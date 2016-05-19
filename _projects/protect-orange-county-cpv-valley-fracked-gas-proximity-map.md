---
layout: project-page
title: "Protect Orange County: CPV Valley Fracked Gas Proximity Map"
linkname: protect-orange-county-cpv-valley-fracked-gas-proximity-map
author: "Chrissy Remein"
tagline: "This is a proximity map for the communities surrounding the CPV Valley Fracked Gas Power Plant. "
location:
    - place: Orange County, NY
project-link:
    - href: https://chrissyremein.github.io/orangecountyprox/map.html
tags:
    - tag: Protect Orange County
    - tag:  Fracked Gas
    - tag:  Fracking NY
thumbnail-path: img/protect-orange-county-cpv-valley-fracked-gas-proximity-map/u98kcx5.jpg
img-folder: ../../img/protect-orange-county-cpv-valley-fracked-gas-proximity-map/
timestamp: 5/15/2016 17:07:26
---
Background:  Protect Orange County is a community action group of concerned citizens working to prevent the CPV Valley Fracked Gas Power Plant from being built. Although fracking is illegal in the State of New York, because of the health and environmental hazards therein- processing of these chemicals is not illegal. The proposed plant would emit harmful carcinogens, neurotoxins, and endocrine disruptors into the atmosphere, as well as loading in 2.1 million tons of green house gasses annually.

There is currently on ongoing federal probe/ investigation on the ‘unusual circumstances’ surrounding the approval of the plant. 

Protect Orange County requested that I make an impact map for the plant site for the surround community.

This is the organization webpage: ![]({{ page.img-folder }}bQojg3Q.jpg)

Map Goal: The goal of the map is to show the health and environmental impacts the plant will have on the surrounding community members. Because the plant is highly volatile, people within 1.5 and 5 miles face are in eminent danger in the event of a plant explosion. The company that owns the plant, had a similar plant in Minisink, NY that exploded and killed 6 people injuring 2. The blast was felt 40 miles out- the harmful chemicals released- are not considered dissipated and not harmful until the 40 mile buffer. The map aims to allow people in the community to see where they are within this context, and also garner more supporters.

The Map Data: In order to complete the map, I used U.S. tax parcel shapefiles of surrounding New York, counties to locate the future proposed plant sight and the surrounding counties of the site including Orange, Ulster, Westchester, Sullivan, and Putnum. I created a shapefile polygon of the plant site. I ran buffers from the plant site from the sat 30,15,5, and 1.5 files, then dissolved that into one shape file. Each of these datasets was organized differently-and some, in separate shapefiles there in. I paired down each dataset to include the bare minimums, County Name , Municipality, size. 

Once the data sets were similar, I ran near tables on each of them, to determine their proximity to the plant location. In order to upload these to CartoDB I had to save the data into 4 shape files. ![]({{ page.img-folder }}ACjpDJn.jpg)

I then uploaded a shape file I made of a remaining data set.
![]({{ page.img-folder }}TDFgCGA.jpg)

To Build an Interactive Online Map: I Uploaded my map to CartoDB. I then added in an interactive sidebar to represent the buffer zones of proximity. Each list item opens to explain the dangers of the proximity.
 ![]({{ page.img-folder }}QmFC5Zw.jpg)


I made this sidebar interact with the map. In this way people have the ability to click on a sidebar item and then see where in the map the are specifically corresponds.
![]({{ page.img-folder }}QmFC5Zw.jpg)

This side bar involved calling in specific data layers through the list item and buttons for each proximity separately.
i.e. 

{% highlight javascript %}
   $('.buffer-30').click (function () {
    $(this).toggleClass('active');
    if ($(this).hasClass('active')) { 
     var sql = "SELECT * FROM finalbuffers WHERE buff_dist =  '48280.4165608'";
    }
    else {
     var sql = "SELECT * FROM finalbuffers";
    }
    dataLayer.setSQL(sql);
   });
{% endhighlight %}

I also added in a pop up with an image and information regarding the plant site- as every Saturday the organization meets in action at the proposed plant site. ![]({{ page.img-folder }}eTxVJI0.jpg)

There is also a line item with information on data permissions and a link to their source.

And a link item link to return to the organization webpage.

The map is simple, but it effective in allowing community members to better understand their proximity to the site, and the health and environmental concerns within.



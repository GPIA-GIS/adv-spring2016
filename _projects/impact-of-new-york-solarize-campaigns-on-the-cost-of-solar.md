---
layout: project-page
title: "Impact of New York Solarize Campaigns on the Cost of Solar"
linkname: impact-of-new-york-solarize-campaigns-on-the-cost-of-solar
author: "Jansyn Thaw"
tagline: "This map identifies the financial impact of group purchasing for residential solar energy systems in New York State."
location:
    - place: New York State
project-link:
    - href: http://jansynthaw.github.io/NYSERDA/
tags:
    - tag: solar
    - tag:  energy
    - tag:  environment
    - tag:  New York
    - tag:  affordability
thumbnail-path: img/impact-of-new-york-solarize-campaigns-on-the-cost-of-solar/NdWsvno.jpg
img-folder: ../../img/impact-of-new-york-solarize-campaigns-on-the-cost-of-solar/
timestamp: 5/16/2016 18:04:20
---
The New York State Energy Research and Development Authority (NYSERDA) is trying to make solar energy more affordable to residents and businesses. In 2014 the state announced Reforming the Energy Vision (REV), which is Governor Cuomo’s comprehensive energy strategy for New York. Cuomo has made a commitment that 50% of New York State’s electricity will be sourced from renewable energy sources by 2030.

My client, NYSERDA, is working to make it easier and more affordable to install solar energy through community-driven initiatives, including Solarize Campaigns, which are what my map show. Solarize campaigns are locally organized community outreach efforts aimed at getting a critical mass of homes and businesses to go solar. When groups of residents and businesses attempt to go solar together, they can reduce the costs of install.

In 2015, communities across New York launched more than 30 Solarize campaigns. Hundreds of households and businesses are going solar as a result. Building on this success, the second round of Solarize campaigns launched in spring of 2016. 

The purpose of this map is to assist NYSERDA in identifying the financial impact of group purchasing for residential solar energy systems, as well as areas of opportunity for future Solarize Campaigns. 

In order to create the map, I pulled data sets from NYSERDA’s internal database, as well as income data from the Department of Housing and Urban Development, and created my own data sets using information from Energize NY and Sustainable CUNY.

After cleaning and organizing the data sets, I geocoded my data using QGIS and GPS Visualizer and joined it to county and municipal-level polygons. I uploaded those shapefiles to CartoDB, where I styled the data and created infowindows and legends.

I built this webpage (hosted in a GitHub repository) using HTML, CSS, and jQuery. I used SQL to link data from my CartoDB visualization to the various checkbox and dropdown options. I also used Bootstrap, Google Fonts, and a CartoDB publishing template I found on GitHub.

<iframe width="100%" height="520" frameborder="0" src="https://thenewschool.cartodb.com/u/jansynthaw/viz/348f3bfa-fda8-11e5-835d-0e3ff518bd15/embed_map" allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>

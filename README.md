# Welcome to the Green Coding Berlin repository for Links, Documents and Resources

# Blogs
- [Microsoft Sustainability blog](https://devblogs.microsoft.com/sustainable-software/feed/)
- [Green Software Foundation Blog](https://greensoftware.foundation/articles)

# Articles
- [OLED power consumption smartphones](https://www.youtube.com/watch?v=D-spTjqAswA&t=3324s)
  + OLEDs consume less energy on red colors and and in dark mode. But negligeable and if movement occurs it is gone
  Smartphone WIFI consumes most wattage. But it may take the least amount of time! So WattH is smallest!
- [Memory Consumption of Browser Extensions](https://www.debugbear.com/blog/chrome-extension-performance-2021#browser-memory-consumption)

# Software

## Desktop software
- [Green IT – Wie wird Ressourceneffizienz von Software klassifizierbar? | jambit CoffeeTalk](https://www.youtube.com/watch?v=NQM-N1g456Y) 
  + Very good talk about UBA study. A bit old-fashioned german style but high quality.
- https://media.ccc.de/v/36c3-10852-wie_klimafreundlich_ist_software#t=2174
  + Different version about same topic from CCC
- https://www.youtube.com/watch?v=NQM-N1g456Y
  + Even different version in a very good german talk, that tries to also include international certificates like epeat etc.
- https://www.umweltbundesamt.de/publikationen/entwicklung-anwendung-von-bewertungsgrundlagen-fuer 
  + Original UBA Talk

## Code Measurement Tools
- [Texas State Marcher Web-Interface to run code in many programming languages and get resource usage metrics](https://greencode.cs.txstate.edu/)

## Linux
- "Linux Power Tools"
- Turbostress

## Windows
- E3 - https://devblogs.microsoft.com/sustainable-software/measuring-your-application-power-and-carbon-impact-part-1/

## Wifi / Cellular-Data Power consumption
- https://github.com/rtslab/EnergyBox


## Carbon removal companies
- https://climeworks.com/

## Academic Research
- https://greenlab.di.uminho.pt/ - Portugal
- [Texas State Green Software Department](https://greensoft.cs.txstate.edu/)

## Web Tools / Services

- [Carbon clock](https://conf.researchr.org/series/ict4s)
- [EnRoads Tool](https://en-roads.climateinteractive.org/scenario.html?v=22.1.0)
  + Tool developed by Climate Interactive in Coop with MIT
  + Mainly build as a showcase and education tool to simulate climate policies
  + Basic display is Energy Sources and GHG Emissions and Temperature Rise
  + You can see many graphs and levers. But before every model it makes sense to dive into the "assumptions".
  + Free Courses to spread the word: https://learn.climateinteractive.org/
- [Electricitymap.org](https://electricitymap.org)
  + See the current CO2 intensity of the grid
- [FlexiDAO](https://www.flexidao.com/)
  + See if your current electricity is Green. Down to energy provider level. And also including matching with vendors.

## Cloud Emission
- [Etsy Cloud Jewels](https://www.etsy.com/codeascraft/cloud-jewels-estimating-kwh-in-the-cloud)
  + First to introduce concept
  + Data coming from SPECPower and 2016 US Data Center Energy Usage Report
  + Model includes idle wattage
  + 2.10 Wh per vCPUh [Server]
  + 0.89 Wh/TBh for HDD storage [Storage]
  + 1.52 Wh/TBh for SSD storage [Storage]
  + No coefficients for RAM and Network. Neglected for now.
  + Cloud Service Products like BigQuery, BigTable: cannot handle.
  + Methodology is Multi-Cloud, but [Github Tool](https://github.com/etsy/cloud-jewels) only works for GCP
- [Greenpixie](https://greenpixie.com/blog/cloud-emission-calculation-methodology-AWS)
  + Based also on billing data
  + Model includes idle wattage
  + Includes Network. But only between datacenters and not to end user. 0.001 kWh/Gb
  + Compute seconds are known. But not utilization. Thus high uncertainty especially for small compute times
  + To get the carbon coeffcients of the servers it uses SPECPower, Etsy Cloud Jewels and 2016 US Data Center Energy Usage Report
  + Handles GPU power in the same way TEADS does
  + Can handle AWS Lamda Service through custom formula that assumes linearity of memory and and vCPUs
  + Can estimate AWS Aurora
  + Other cloud services from Amazon like DynamoDB it cannot handle
  + Estimates storage based on 2016 US Data center report. 0.65 W / TB for HDD;  1.2 W/TB for SSD
  + Uses [replication factors for storage and database](https://docs.google.com/spreadsheets/d/1D7mIGKkdO1djPoMVmlXRmzA7_4tTiGZLYdVbfe85xQM/edit#gid=735227650)

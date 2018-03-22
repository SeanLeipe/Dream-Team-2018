# Helping Hand - by the Dream Team

## ECCE App Challenge 2018

### Team Members
Mark Borthwick, Jayden Choi, Sean Leipe, Chandler Podhorodeski

# Mission Statement

Life in Canada’s largest city is rarely easy with an unfortunate one in five Toronto residents currently living in poverty. For those struggling to make ends meet, it can be difficult to secure all necessities of western life such as sufficient nutrition, educational resources, and shelter on a daily basis. Currently, many government and private services exist in Toronto that aim to assist low-income residents in one or more areas. The issue is that all too often those in need do not realize these services exist, let alone where to access them until their situation becomes dire.

**Helping Hand's goal** is to create an easy-to-use tool that consolidates community resources for at-risk or lower-income families in Toronto, based on open geospatial data hosted by the city. These resources include public libraries, licensed child-care services, youth services, supportive housing locations, and more (a full list is under the **Data Sources** section). This app gives a convenient way to either find specific locations through a search based on their name, street address, etc., or by giving a full list of all the different resources available with a specified distance of a location.

# User Guide

## Getting Started

### *Using ArcGIS Online*
Click the link below to access our app through ArcGIS Online!

### *Using the WAB Developer Edition*
1. Download the *app.zip* file from the repository and extract its contents.
2. Navigate to the *webappbuilderforGIS* file.
3. Click on the *startup.bat* file, which will open a link in your browser.

If any problems come up, check out the [Esri Web App Builder FAQ](https://developers.arcgis.com/web-appbuilder/guide/faqs.htm) documentation.

## Explore Resources
Use the *Layer List* button on the top right to go through the list of available community resources. Simply check the box next to the desired resource to control what shows up as icons on the map. You can see what each icon represents through the nearby *Legend* button.

## Find Specific Resources
Click on the green Query button to open a drop-down menu, and select the type of resource you want to search through. You can then search for specific locations through their name, address, or other characteristics. Clicking on one of the results creates a pop-up with more information on the resource.

## Find Nearby Resources
Click on the blue *Nearby* widget at the bottom of the screen, and either enter your address or click on the map. Use the slider below to decide how far of a distance from your location you want to find resources in.

After selecting the distance, the tool will give you a list of all the community resources close to you, separated by type. Clicking on a resource type will give you a list of all their locations within the given distance, in order of closest to farthest. Clicking on an individual resource will open up a pop-up with more information about the facility such as its street address, phone number, email address, and more.

For driving directions to your desired location, simply click on the *Directions* tab and step-by-step instructions will show up in the tool window. These can be printed out for reference by using the Print icon in the top right corner of the pop-up.

For walking directions, copy the open the address given from either the *Nearby* or *Query* results and open the orange *Directions* widget. Set your start point, paste the address as the end point, and select Walking Directions from the drop-down list.

# App Characteristics

This app creates an easy way to explore community resources in Toronto

Though any of these specific locations could be found using a Google search, this app lets you explore any of the 10 different resource types, 

## Data Sources

This app was designed using the Developer Edition of the ArcGIS Web App Builder.  All data used was obtained from the [City of Toronto’s open data portal](https://www.toronto.ca/city-government/data-research-maps/open-data/). Feature layers were either downloaded directly as point shapefiles, or converted to points from CSV files using their listed x-y coordinates. The different feature layers representing community resources used in the app are:

* Public libraries
* Long-term care facilities
* Rent banks
* Licensed child-care services
* Air-conditioned public places
* Homeless shelters
* Youth services centres
* Drop-in locations
* Supportive housing locations

For some of the point layers, key attribute information such as names, email addresses, websites, etc. were either unavailable or formatted incorrectly. This issue was corrected using Arcade expressions with conditional logic.

## Widgets Used

The web app interface uses the following widgets:

* **Splash screen**: to introduce the user to the app
* **Share**: gives a shareable link to the web app on ArcGIS Online
* **Layer List**: to let the user control which layers are visible 
* **Legend**:
* **Query**: to search for specific resources
* **Nearby**: to find resources within a specific distance of and obtain information and driving directions
* **Directions**: to get walking directions for a specific resource

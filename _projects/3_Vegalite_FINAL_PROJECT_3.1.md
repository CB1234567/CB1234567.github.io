---
name: Final Project Part 3.1 Group 7
tools: [Python, HTML, vega-lite, Altair,Jekyll, interactive]
image: assets/pngs/cars.png
description: This is the first part of the final group project part 3.1.It uses vega-lite and Altair for interactivity. Group members include Chetna Beri, Aatmic Tiwari and Sankalp Jain.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---
# Light, Camera, Location aanndd....Action!!
## Final Project Part 3.1, Group - 07
### An interactive analysis of shooting locations in New York City. 
## Team Members: 
#### Chetna Beri
#### Aatmic Tiwari
#### Sankalp Jain

The art of filmmaking is exciting and challenging. From saying the four (in our case five) magical words to assembling costumes, locations, script, acting, directing and everything that lies in between it takes decades if not years to master. In our analysis today, we will be looking at one aspect mainly the shoot location and some formal permissions and procedures that lie in this realm. Our dataset is collected and maintained by the New York State Department’s Mayor’s Office of Media and Entertainment (MOME). Our dataset is in public domain and has 10.8 downloads, 13.6K rows and 14 columns where each row is a film permit giving us information about the location, borough, date and time of the permit etc. We have created our own graphs for both the main as well as the contextual visualizations.

# Visualization 1: Interactivity in Focus
## Understanding Interactivity through Altair
We have also presented an interactive dashboard displaying the total days allocated to an event. The graph is a simple pie chart showing the percentage breakdown of each event type. Users can switch and choose from the graph legend to analyze trends, correlations, and patterns. This allows for easy comparison between different event types. The interactivity of this dashboard makes it easy to visualize and understand the data presented. By analyzing this data, we can gain insights into which event types are most popular and how long permits are typically issued for each type of event. 


```
The following graph is made interactive by clicking on the legends. Upon clicking the legends. Click outside the legend to return to original state.
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/FP_Chart1.json" style="width: 100%"></vegachart>

This data can be useful in a variety of ways, such as helping production companies plan their shoots more effectively and efficiently or assisting city officials in allocating resources to support the film industry. In addition, the data can be used to explore patterns and trends over time, which can help identify opportunities for growth or areas where improvements can be made.
The given contextual data (Link: https://data.cityofnewyork.us/City-Government/NYC-Permitted-Event-Information/tvpp-9vvx) is a more in-depth form of the data we use in our project. As we mentioned, we are using that data in which different types of events are being listed and which area exactly they have to hold the parking, do barricading or provide police enforcement. But, this contextual data considers only circumstances involving more than one street for the event and those that will continue for at least five days and few other countries like Canada,UK are also being involved in this. This will give more insights into those spots which are being used more frequently and are the most popular spots as compared to New York City with specific boroughs.


#  Visualization 2: Analysis from Contextual Data
## Understanding the dataset by performing primary analysis and plots.
Our initial analysis started with understanding the spread of data within the columns for the contextual and original datasets. In this section we have explored contextual dataset analysis. In the previous assignment we have worked on the main dataset. This meant that we plotted simple yet effective bar plots using python libraries like seaborn and matplotlib. From this we understood that sports and youth events are highest with respect to event type and a number of other events are lowest. The data is found to be consistent as both the category column and the sub-category column seem to follow a similar pattern. We have eventually dropped the Country column as over 95% of the columns belong to same country. Furthermore, we have analyzed Borough data using stacked barcharts. We have found that Staten Island and Manhattan have the lowest and highest number of shooting permits being granted and seem to be popular locations among movie makers. This leads us to believe that perhaps Manhattan is more familiar to audiences as compared to Staten Island which doesn seem to be the obvious choice for filmmakers. Brooklyn at number feels like a popular choice because of obvious landmarks like the Brooklyn bridge which we see in a lot of movies and TV series. It is also a lot cheaper than NYC Central like Manhattan and Times Square. We do not have ample data to support us for Times Square and Central Park and hope that in future the government presents us with the opportunity to analyze this by making the data public.

```
Plotting count of Categories for every category. We have performed this for other graphs as wee for our understanding but presented two.
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/FP_Chart2.json" style="width: 100%"></vegachart>

<vegachart schema-url="{{ site.baseurl }}/assets/json/FP_Chart3.json" style="width: 100%"></vegachart>


## Challenges
While plotting the graphs and uploading to github we faced numerous challenges as the file size was larger than supported. Hence we have included specific code like 
alt.data_transformers.enable('default', max_rows=None)
and also made use of nbviewer for viewing the data uploaded in github. This allows us to view data. At the same time working with Altair was challenging as there is minimal support and the library is basic. Interactivity is hard to achieve but it is interesting to work with.


## Conclusion
Overall, the use of data from the Film Permits dataset has allowed us to build powerful visualizations that make it easier to explore and understand trends in the film industry in New York City.




<div class="left">
{% include elements/button.html link="https://data.cityofnewyork.us/City-Government/Film-Permits/tg4x-b46p" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://nbviewer.org/github/CB1234567/CB1234567.github.io/blob/main/Group_7_Final_Project_Part3.1.ipynb" text="The Analysis" %}
</div>

<div class="centre">
{% include elements/button.html link="https://data.cityofnewyork.us/City-Government/NYC-Permitted-Event-Information/tvpp-9vvx" text="Contextual Data" %}
</div>



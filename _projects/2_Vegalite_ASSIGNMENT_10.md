---
name: ASSIGNMENT 10
tools: [Python, HTML, vega-lite, Altair]
image: assets/pngs/cars.png
description: This is Assignment 10 which uses vega-lite and Altair for interactivity.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# Homework - 10, Group - 36
## Team Member: 
#### Chetna Beri

#### In this assignment we have learnt to use Vegalite, Python and Altair for plots. I have made use of the same dataset as Assignment 9. It has certain information about Buildings, like the year of construction and number of rooms, floors etc. I have constructed two visualizations using this data. The first visualization makes use of tooltip and the third one makes use of dropdown menu to select the year whose data needs to be displayed. I have tried to make the data as simple and understandable as possible as I believe that simple visualizations make good visualizations.


# Visualization 1
## Understanding the relationship of square footage and Total floors.
Through this graph I have tried to understnad the relationship between the square footage and total number of floors in the building. It can be observed that major data lies between 0 to 300,000. This is quite possible as it is rarer to find buildings with larger houses especially in citites. We cannot derive any direct relationship between swuare footage and floors. Data seems to be arbitarily distributed and does not follow any sort of fixed pattern.

I have made use of the tooltip here and the graph changes color on being clicked for tootltip. The second graph is more interactive. The color changing ability is made possible using colormap.I have made use of the .properties function to set width and height of the map. I have also made use of brush selector and x and y flatten transform. The color encoding changes the g=color from green to blue on being selected. The **from_dict()** function helps us use our own data.  


```
<vegachart schema-url="{{ site.baseurl }}/assets/json/Chart1.json" style="width: 100%"></vegachart>
```

<vegachart schema-url="{{ site.baseurl }}/2_Vegalite_ASSIGNMENT_10.md" style="width: 100%"></vegachart>

# Visualization 2
## Understanding the relationship of square footage and Year Constructed.
Through this graph I have tried to understnad the relationship between the square footage and the year in which the building was constructed. I have used .properties and **select_box** tool for selecting dates froma dropdown menu. The **.properties** allows me to set the size of the graph. I have also used **tooltip and color encoding** to denote changes in color when graph is selected. This graph is truly interactive. I really enjoyed making this graph as it was challenging and exciting to learn something new and execute it. I have performed sum aggregation in order to display the sum of square foots along the year. I have used a horizontal bar chart for this graph.

As we can see there is almost a parabolic curve like relationship between swuare footage and years constructed. As the years increase the quarefootage increased and then led to a gentle fall in the square footage as well. The last part of the fall can also be due to lack to data in the recet years and plenty of descriptive data in the previous historical years. 


```
<vegachart schema-url="{{ site.baseurl }}/assets/json/Chart2.json" style="width: 100%"></vegachart>
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/Chart2.json" style="width: 100%"></vegachart>


<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/CB1234567/CB1234567.github.io/blob/main/Beri_Chetna_ASSIGNMENT_10.ipynb" text="The Analysis" %}
</div>


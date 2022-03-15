<div>
<img width = "100%" align="center" alt="PIC" height="400px" src="https://github.com/GODZAOZAO/optimal-bus-lane/blob/main/chicago_bus.jpeg" />
<div/>
  
# Chicago Optimal Bus Lanes
To increase the usage of bus lanes and improve traffic flow, this model predicts the performance and benefits of bus lanes on busy road segments in the City of Chicago.

## Getting Started
* Use Google Colaboratory / jupyter notebook to analyze Chicago traffic datasets 
  - https://github.com/GODZAOZAO/optimal-bus-lane/blob/main/IUP%20Project.ipynb
~~~python
# Important library for many geopython libraries
  !apt install gdal-bin python-gdal python3-gdal 
  
# Install rtree - Geopandas requirment
  !apt install python3-rtree 
  
# Install Geopandas
  !pip install git+git://github.com/geopandas/geopandas.git
  
# Install descartes - Geopandas requirment
  !pip install descartes 
  
# Install Folium for Geographic data visualization
  !pip install folium
  
# Install plotlyExpress
  !pip install plotly_express
  
!pip install pygraphviz --install-option="--include-path=/usr/include/graphviz" --install-option="--library-path=/usr/lib/graphviz/"
from networkx.drawing.nx_agraph import graphviz_layout
~~~
  
## Key Features
* Data Preprocessing
  - Uses haversine formula to calculate distance between two lat long points
  - Splitting necessary as a road segment may not stop at every intersection
  - Manages the list of nodes associated with a street
* Visualization of the Entire CTA Bus Network
* Visualization of Segments With Chicago Traffic Congestion Data
* Use Activity and Gravity Score to Evaluate Traffic Congestion
  
<img src="https://github.com/GODZAOZAO/optimal-bus-lane/blob/main/Activity%20Score.png" width="500" height="100"/> <img src="https://github.com/GODZAOZAO/optimal-bus-lane/blob/main/Gravity%20Score.png" width="500" height="100"/>
  
</p>
 
  
## Results
<img src="https://github.com/GODZAOZAO/optimal-bus-lane/blob/main/Congestion_Chicago.png" width="500" height="600"/> <img src="https://github.com/GODZAOZAO/optimal-bus-lane/blob/main/All_Traffic_Chicago.png" width="500" height="600"/>


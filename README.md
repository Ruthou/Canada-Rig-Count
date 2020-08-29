# Canada-Rig-Count
Public Data Set 
---Power BI Report
By Ruth (Ying) Hou
•	Brief Introduction
•	Public Data Source
•	Analysis & Visualization Tools 
•	BI Results and Analysis
•	Conclusions

Brief Introduction
Rig count is a strong indicator to see how active drilling activities are, and a significant implicit barometer of how the whole oil & gas industry performs since this upstream section generates the highest margins most of the time. It may also serve as a prediction to the investments movements in this industry. 
Oil industry is strongly cyclical. The main purpose of this ‘Canada Rig Count’ BI project is a brief proof of this cyclical industry; identify the seasonal land rig activities of Western Canada; notify that Alberta is a major player among all the 13 provinces and territories of Canada which has drilling activities; and try to track the trend of Alberta drilling activities and see if COVID-19 has extra influence for this market, or if we are able to see a recovery coming on the way.
Public Data Source
The open data is coming from an excel table named “North America Rig Count by Bake Hughes” (https://rigcount.bakerhughes.com/na-rig-count), extracted one sheet only, called “Canada L & OS Split by Province”.
Analysis & Visualization Tools
Power BI & Zebra BI
BI Results & Analysis
 
Tile 1 
This first graph is an overview of weekly rig counts since 2003 in Canada. There are all together 13 provinces and territories which has active drilling activities in Canada. Western Canada, including Alberta, Saskatchewan, BC, and Manitoba are the main players. I have the rest of the provinces and territories grouped as others. 
For Alberta, you may notice that drilling activities dropped more than half since 2015 from its peaks in 2006, 2007, 2008 and 2012. 
Also, you may notice, there are cyclical dips every year, the shorter span dips usually happens during Christmas breaks; the longer span ones, which usually starts dropping from end of March, and starts to pick up from the end of May, generally last about two to three months. 
This long-term dip is called “spring breakup”, which describes the time of year when the oil industry, specifically across western Canada, slows down due to the melting snow and frost that causes the ground to become soft and muddy, which is unsafe for the heavy drilling equipment trucking in or out. And unfortunately, this is also a time you see manpower dropping in this industry in Western Canada.
Besides, some dips are particularly wider, which means drilling activities resumed slower than a normal spring breakup required. To my understanding, 2009 wider dip was a result of the post-reaction to US Financial Crisis; the wider dips of 2016 and 2019 were a result of industry recession. We probably will foresee another wider dip for 2020 due to COVID-19 and global recession. 
 
Tile 2
This tile shows how each province weighs in drilling.
This pie chart tile has dynamic title and can be filtered by time slicer. From this tile, we can see that Alberta has been the No.1 player ever since we record this count. If you filter the years, you may realize that Alberta used to weigh over 70% of drilling activities across whole Canada. Yet, it started to weigh less since 2008, and BC and Saskatchewan had caught up since then. 
 
Tile 3
This is a sunburst chart you can load from ‘more visuals’ and added to your visualization inventories. It looked like another pie chart, yet you can group more dimensions here. In my case, I have quarters and provinces grouped together. Filter by year and provinces, you will be proved again that Quarter 2 is the low season for all Western Canada with land rig activities. But offshore rigs reflected in ‘others’ is not influenced with seasons. Instead, they are steady all year around.
 
Tile 4
Tile 4 reflects the relationship between land rig activity and offshore rig activity. Land rig activities overweighs with activities fluctuations, while offshore activities keep steady yet weighs not much at all. Filtering by provinces, you can have a breakdown graph of Tile 1 by each province.
 
Tile 4 & 4A
Lastly, let us show some trend analysis. This is Alberta trend analysis. Left tile 4 is generated in Power BI, and right tile 4A in Zebra BI. Since Alberta weighs about 70% of rig activities, it can be a good representative of whole Canada. 
The trend line in Power BI is not aligned to the shapes formed by the columns representing the rig activities by the given years. If you look at the trend analysis closely, you will see the peaks and lows of the trend line did not spot on the correct positions. 
It seems that Power BI trend line directions (up or down) change earlier when forecasting an opposite direction change in the next following year (the time frame you defined) and pre-acts to that forecast. Neither shape nor proportion is this trend line convincible. 
On the contrast, Zebra BI has its trend shape and proportion aligned to the analysis numbers; the peaks, lows and turns are positioned correctly. Obviously, Zebra BI works a better job here.
Conclusions
There are a couple of takeaways from my projects.
First, my open data set has dual headers. I was guided to do “unpivot table” to recategorize my dimensions, split the columns of values with new established dimensions, till a normal fact table presents.
Second, Dim Date table is mandatory to almost every data set. I am able to pick up some essential DAX language to create a data table with some calculated columns.
Third, Bake Huges’ weekly rig count is my only value measure in Fact table. It is an industry acceptable measure of drilling activities and is not necessarily linked to wells or actual drilling time. And granularity to weekly is also just a detailed enough portrait of rig activities. I choose to use ‘Yearly Average’ more to do the aggregation function, reflecting the low granularity measures.
Fourth, Zebra BI has a more convincing trend visual. Will need further research on how the trend line coded and plotted in Power BI.



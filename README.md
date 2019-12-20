# Open-Data-2019 
Documentation on data analysis:

Here are the steps of data management we followed using QGIS 2.18 software:

I. Selection of the prefecture M’Boi Mirim inside the São Paulo administrative borders

II. Selection inside the prefecture M’Boi Mirim using ‘spatial query’ tool of:

a. census tracts

b. landslide risk areas

c. favelas

III. Intersections of data:

a. Prefecture M’Boi Mirim census tracts and landslide risk areas ⇒ basic statistics for people in risk → Field calculator:

Pop in risk = (risk_area * prefecture_pop) / prefecture_area

b. Prefecture M’Boi Mirim census tracts and favelas* * layer with error that required fix through ‘verify validity’ tool ⇒ basic statistics for people living in favelas → Field calculator:

Pop in favelas = (fav_area * prefecture_pop) / prefecture_area

c. Prefecture M’Boi Mirim census tracts and landslide risk areas and favelas ⇒ basic statistics for people living in favelas in risk → Field calculator:

Pop in favelas in risk = (fav_risk_area * prefecture_pop) / prefecture_area

IV. Categorization of data:

a. Population density by census tracts

b. Population density by favelas in risk

c. Levels of landslide risk ⇒ basic statistics for people living in risk by levels of landslide risk

d. Special Areas of Social Interest (ZEIS) ⇒ basic statistics of ZEIS by type (2, 4 or 5) ⇒ From the area available for social interest (ZEIS), we calculated the number of people that could be relocated and compare with the number of people in risk (both in favelas and in other areas with infrastructure)

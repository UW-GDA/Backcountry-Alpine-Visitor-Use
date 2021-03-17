# Backcountry-Alpine-Visitor-Use

### Introduction/Problem Statement

The population of the Western US has gorwn markedly in the last 10 years, especially in Western Washington. This growth has translated into increased reacreation within the National Forests and the three National Parks found within Washington's borders. As use increases, documentation of the degredation of these wilderness areas has increased, but the possible contribution of remote sensing using satellinte imagery and LIDAR have yet to be explored. Social trails, common in alpine areas, have long been used by visitors to connect and create campsites as well as navigate topology. It is posited, as visitation rates grow, social trail use will also intensify, compacting alpine soils, killing plants and expanding the breadth of previously established trail networks. This project will evaluate the feasibility of using the National Agriculture Imagery Program (NAIP) and the social trails in alpine wilderness areas in Washington State. If plausible, polygons will be used to capture social trail expanse and track it over time.

### Approach

Use 4-band NAIP data because of the 1m resolution. Each band will be investigated for its plausibility in quantifying social trails. If possiblle, annual comparisons will be made to see if the overall area of social trails increases over time.


### Team Members

* Gabriel Wisswaesser

### Examples of Imagery to Be Ivestigated

### Rampart Lakes RBG

<img src="rbg.png" width=50% height=50%>

<br>

### Rampart Lakes Red/Blue

<img src="rbr.png" width=50% height=50%>


### Product

* A notebook with investigator steps into feasability of using rasters to measure social trails

### Python Packages
* imageio
* matplotlib
* numpy
* os
* Rasterio
* urllib

### Directory Structure
.
├── LICENSE <br>
├── README.md <br>
├── m_4712138_sw_10_1_20110826.tif<br>
├── m_4712138_sw_10_1_20110826_utm_gdalwarp.tif<br>
├── m_4712138_sw_10_1_20150807.tif<br>
├── m_4712138_sw_10_1_20150807_utm_gdalwarp.tif<br>
├── rbg.png<br>
├── rbr.png<br>
├── research.ipynb<br>
├── robin-lakes-social-trail<br>
│   ├── 01-robin-2013.jpg<br>
│   ├── 02-robin-2014.jpg<br>
│   ├── 03-robin-2015.jpg<br>
│   ├── 04-robin-2017.jpg<br>
│   ├── 05-robin-2018.jpg<br>
│   └── robin-lakes.gif<br>
└── robin-lakes.gif<br>

# Conclusions

* Red band was the best
    * normalization added rocks (high sensitivity, low selectivity)
    * r/b ratio removed rocks, but lost other sections of social trails and added others (mid sensitivity, low selectivity)
    * 
* Compare between years
    * Hard to compare between years
      * precip differences
      * photos taken at different times of day
      * vegetation casts shadows

* Might be useful under different expectations and conditions
    * True alpine or open space with no tall vegetation
    * Photos were same day and time of each year
    * use imagery to determine impervious to semi-impervious surfaces instead of only social trails
        * This would combine rocks and open soils (compacted from trails included). Possible difference in area between years could be increasing social trails as rocks likely to                                    remain the same


### Data Source

*https://earthexplorer.usgs.gov/

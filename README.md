# Chicago Crime Data from 2001 to present


This repo contains a data set from the Chicago Police department for crimes committed between 2001 to the present(with the exception of murders where data exists for each victim). This project is dedicated to doing some cool data analysis and visualization on this already curated dataset.

Data visualizations were created through the super awesome Python library **folium**, which I highly recommend to make beautiful map visualizations.

Some visualizations were not able to render properly in jupyter notebook, but I have saved all of the visualizations (and some more) as html files in the [visualization](https://github.com/k-chuang/Chicago-Crime-Data-Analysis/tree/master/visualizations) folder.

There are some more in depth visualizations located in that folder as well, such as all Chicago crimes reported in 2018 so far. Descriptions of each map visualization is shown below:

* [2018-chicago-crimes.html](https://github.com/k-chuang/Chicago-Crime-Data-Analysis/blob/master/visualizations/2018-chicago-crimes.html): This map is a detailed map visualization of all the crimes commited in Chicago from Jan. 1, 2018 to March 19, 2018, with popup markers that display more information about each individual map, such as date, time, location, crime type, and crime description.
* [2018-chicago-crime-heatmap.html](Chicago-Crime-Data-Analysis/visualizations/2018-chicago-crime-heatmap.html): This map contains a heat map of all the crimes commited in Chicago from Jan. 1, 2018 to March 19, 2018.
* [March-2018-chicago-crimes.html](Chicago-Crime-Data-Analysis/visualizations/March-2018-chicago-crimes.html): This map is a detailed map visualization of all the crimes commited so far in the month of March (March 1, 2018 to March 19, 2018), with popup markers that display more information about each individual map, such as date, time, location, crime type, and crime description.
* [March-2018-chicago-crime-heatmap.html](Chicago-Crime-Data-Analysis/visualizations/March-2018-chicago-crime-heatmap.html): This map contains a heat map of all crimes commited so far in the month of March (March 1, 2018 to March 19, 2018).
* [Crime-per-district-choropleth.html](Chicago-Crime-Data-Analysis/visualizations/Crime-per-district-choropleth.html): This map contains a choropleth map of all the crimes from 2001 to present (March 19, 2018) based on [Chicago Police District](https://data.cityofchicago.org/d/fthy-xz3r)

Also, here is the nbviewer for my jupyter notebook where most of the maps are rendered (the visualization occasionally doesn't show up in Chrome, but does show up on Firefox or Safari): [Notebook Viewer](http://nbviewer.jupyter.org/github/k-chuang/Chicago-Crime-Data-Analysis/blob/master/Chicago-Crime-Data-Analysis.ipynb)



## Description of Columns:
<table class="table table-borderless table-condensed table-discrete schema-table">

<thead>

<tr>

<th scope="col" class="column-name">Column Name</th>

<th scope="col" class="column-description">Description</th>

<th scope="col" class="column-type">Type</th>

</tr>

</thead>

<tbody>

<tr class="column-summary" data-column="id" aria-expanded="false" aria-haspopup="true" role="link" tabindex="0">

<td class="column-name" scope="row">ID</td>

<td class="column-description">

<div class="contents clamped" data-original-height="21" style="height: 100px;"><span class="Linkify">Unique identifier for the record.</span></div>

</td>

<td class="column-type">

<div><span aria-hidden="true" class="icon icon-number"></span><span class="type-name" data-name="number">Number</span></div>

</td>





<tr class="column-summary" data-column="case_number" aria-expanded="false" aria-haspopup="true" role="link" tabindex="0">

<td class="column-name" scope="row">Case Number</td>

<td class="column-description">

<div class="contents clamped" data-original-height="21" style="height: 100px;"><span class="Linkify">The Chicago Police Department RD Number (Records Division Number), which is unique to the incident.</span></div>

</td>

<td class="column-type">

<div><span aria-hidden="true" class="icon icon-text"></span><span class="type-name" data-name="text">Plain Text</span></div>

</td>



</tr>


<tr class="column-summary" data-column="date" aria-expanded="false" aria-haspopup="true" role="link" tabindex="0">

<td class="column-name" scope="row">Date</td>

<td class="column-description">

<div class="contents clamped" data-original-height="21" style="height: 100px;"><span class="Linkify">Date when the incident occurred. this is sometimes a best estimate.</span></div>

</td>

<td class="column-type">

<div><span aria-hidden="true" class="icon icon-date"></span><span class="type-name" data-name="calendar_date">Date & Time</span></div>

</td>



</tr>


<tr class="column-summary" data-column="block" aria-expanded="false" aria-haspopup="true" role="link" tabindex="0">

<td class="column-name" scope="row">Block</td>

<td class="column-description">

<div class="contents clamped" data-original-height="21" style="height: 45px;"><span class="Linkify">The partially redacted address where the incident occurred, placing it on the same block as the actual address.</span></div>

</td>

<td class="column-type">

<div><span aria-hidden="true" class="icon icon-text"></span><span class="type-name" data-name="text">Plain Text</span></div>

</td>



</tr>



<tr class="column-summary" data-column="iucr" aria-expanded="false" aria-haspopup="true" role="link" tabindex="0">

<td class="column-name" scope="row">IUCR</td>

<td class="column-description">

<div class="contents clamped" data-original-height="21" style="height: 65px;"><span class="Linkify">The Illinois Unifrom Crime Reporting code. This is directly linked to the Primary Type and Description. See the list of IUCR codes at [https://data.cityofchicago.org/d/c7ck-438e](https://data.cityofchicago.org/d/c7ck-438e).</span></div>

</td>

<td class="column-type">

<div><span aria-hidden="true" class="icon icon-text"></span><span class="type-name" data-name="text">Plain Text</span></div>

</td>



</tr>



<tr class="column-summary" data-column="primary_type" aria-expanded="false" aria-haspopup="true" role="link" tabindex="0">

<td class="column-name" scope="row">Primary Type</td>

<td class="column-description">

<div class="contents clamped" data-original-height="21" style="height: 100px;"><span class="Linkify">The primary description of the IUCR code.</span></div>

</td>

<td class="column-type">

<div><span aria-hidden="true" class="icon icon-text"></span><span class="type-name" data-name="text">Plain Text</span></div>

</td>



</tr>



<tr class="column-summary" data-column="description" aria-expanded="false" aria-haspopup="true" role="link" tabindex="0">

<td class="column-name" scope="row">Description</td>

<td class="column-description">

<div class="contents clamped" data-original-height="21" style="height: 45px;"><span class="Linkify">The secondary description of the IUCR code, a subcategory of the primary description.</span></div>

</td>

<td class="column-type">

<div><span aria-hidden="true" class="icon icon-text"></span><span class="type-name" data-name="text">Plain Text</span></div>

</td>



<tr class="column-summary" data-column="location_description" aria-expanded="false" aria-haspopup="true" role="link" tabindex="0">

<td class="column-name" scope="row">Location Description</td>

<td class="column-description">

<div class="contents clamped" data-original-height="21" style="height: 100px;"><span class="Linkify">Description of the location where the incident occurred.</span></div>

</td>

<td class="column-type">

<div><span aria-hidden="true" class="icon icon-text"></span><span class="type-name" data-name="text">Plain Text</span></div>

</td>



</tr>



<tr class="column-summary" data-column="arrest" aria-expanded="false" aria-haspopup="true" role="link" tabindex="0">

<td class="column-name" scope="row">Arrest</td>

<td class="column-description">

<div class="contents clamped" data-original-height="21" style="height: 100px;"><span class="Linkify">Indicates whether an arrest was made.</span></div>

</td>

<td class="column-type">

<div><span aria-hidden="true" class="icon icon-check"></span><span class="type-name" data-name="checkbox">Checkbox</span></div>

</td>



</tr>

<tr class="column-summary" data-column="domestic" aria-expanded="false" aria-haspopup="true" role="link" tabindex="0">

<td class="column-name" scope="row">Domestic</td>

<td class="column-description">

<div class="contents clamped" data-original-height="21" style="height: 100px;"><span class="Linkify">Indicates whether the incident was domestic-related as defined by the Illinois Domestic Violence Act.</span></div>

</td>

<td class="column-type">

<div><span aria-hidden="true" class="icon icon-check"></span><span class="type-name" data-name="checkbox">Checkbox</span></div>

</td>



</tr>


<tr class="column-summary" data-column="beat" aria-expanded="false" aria-haspopup="true" role="link" tabindex="0">

<td class="column-name" scope="row">Beat</td>

<td class="column-description">

<div class="contents clamped" data-original-height="21" style="height: 120px;"><span class="Linkify">Indicates the beat where the incident occurred. A beat is the smallest police geographic area – each beat has a dedicated police beat car. Three to five beats make up a police sector, and three sectors make up a police district. The Chicago Police Department has 22 police districts. See the beats at [https://data.cityofchicago.org/d/aerh-rz74](https://data.cityofchicago.org/d/aerh-rz74).</span></div>

</td>

<td class="column-type">

<div><span aria-hidden="true" class="icon icon-text"></span><span class="type-name" data-name="text">Plain Text</span></div>

</td>



</tr>


<tr class="column-summary" data-column="district" aria-expanded="false" aria-haspopup="true" role="link" tabindex="0">

<td class="column-name" scope="row">District</td>

<td class="column-description">

<div class="contents clamped" data-original-height="21" style="height: 80px;"><span class="Linkify">Indicates the police district where the incident occurred. See the districts at [https://data.cityofchicago.org/d/fthy-xz3r](https://data.cityofchicago.org/d/fthy-xz3r).</span></div>

</td>

<td class="column-type">

<div><span aria-hidden="true" class="icon icon-text"></span><span class="type-name" data-name="text">Plain Text</span></div>

</td>



</tr>


<tr class="column-summary" data-column="ward" aria-expanded="false" aria-haspopup="true" role="link" tabindex="0">

<td class="column-name" scope="row">Ward</td>

<td class="column-description">

<div class="contents clamped" data-original-height="21" style="height: 100px;"><span class="Linkify">The ward (City Council district) where the incident occurred. See the wards at [https://data.cityofchicago.org/d/sp34-6z76](https://data.cityofchicago.org/d/sp34-6z76).</span></div>

</td>

<td class="column-type">

<div><span aria-hidden="true" class="icon icon-number"></span><span class="type-name" data-name="number">Number</span></div>

</td>



</tr>


<tr class="column-summary" data-column="community_area" aria-expanded="false" aria-haspopup="true" role="link" tabindex="0">

<td class="column-name" scope="row">Community Area</td>

<td class="column-description">

<div class="contents clamped" data-original-height="21" style="height: 100px;"><span class="Linkify">Indicates the community area where the incident occurred. Chicago has 77 community areas. See the community areas at [https://data.cityofchicago.org/d/cauq-8yn6](https://data.cityofchicago.org/d/cauq-8yn6).</span></div>

</td>

<td class="column-type">

<div><span aria-hidden="true" class="icon icon-text"></span><span class="type-name" data-name="text">Plain Text</span></div>

</td>



</tr>


<tr class="column-summary" data-column="fbi_code" aria-expanded="false" aria-haspopup="true" role="link" tabindex="0">

<td class="column-name" scope="row">FBI Code</td>

<td class="column-description">

<div class="contents clamped" data-original-height="21" style="height: 100px;"><span class="Linkify">Indicates the crime classification as outlined in the FBI's National Incident-Based Reporting System (NIBRS). See the Chicago Police Department listing of these classifications at [http://gis.chicagopolice.org/clearmap_crime_sums/crime_types.html](http://gis.chicagopolice.org/clearmap_crime_sums/crime_types.html).</span></div>

</td>

<td class="column-type">

<div><span aria-hidden="true" class="icon icon-text"></span><span class="type-name" data-name="text">Plain Text</span></div>

</td>



</tr>


<tr class="column-summary" data-column="x_coordinate" aria-expanded="false" aria-haspopup="true" role="link" tabindex="0">

<td class="column-name" scope="row">X Coordinate</td>

<td class="column-description">

<div class="contents clamped" data-original-height="21" style="height: 100px;"><span class="Linkify">The x coordinate of the location where the incident occurred in State Plane Illinois East NAD 1983 projection. This location is shifted from the actual location for partial redaction but falls on the same block.</span></div>

</td>

<td class="column-type">

<div><span aria-hidden="true" class="icon icon-number"></span><span class="type-name" data-name="number">Number</span></div>

</td>



</tr>


<tr class="column-summary" data-column="y_coordinate" aria-expanded="false" aria-haspopup="true" role="link" tabindex="0">

<td class="column-name" scope="row">Y Coordinate</td>

<td class="column-description">

<div class="contents clamped" data-original-height="21" style="height: 100px;"><span class="Linkify">The y coordinate of the location where the incident occurred in State Plane Illinois East NAD 1983 projection. This location is shifted from the actual location for partial redaction but falls on the same block.</span></div>

</td>

<td class="column-type">

<div><span aria-hidden="true" class="icon icon-number"></span><span class="type-name" data-name="number">Number</span></div>

</td>



</tr>


<tr class="column-summary" data-column="year" aria-expanded="false" aria-haspopup="true" role="link" tabindex="0">

<td class="column-name" scope="row">Year</td>

<td class="column-description">

<div class="contents clamped" data-original-height="21" style="height: 100px;"><span class="Linkify">Year the incident occurred.</span></div>

</td>

<td class="column-type">

<div><span aria-hidden="true" class="icon icon-number"></span><span class="type-name" data-name="number">Number</span></div>

</td>



</tr>


<tr class="column-summary" data-column="updated_on" aria-expanded="false" aria-haspopup="true" role="link" tabindex="0">

<td class="column-name" scope="row">Updated On</td>

<td class="column-description">

<div class="contents clamped" data-original-height="21" style="height: 100px;"><span class="Linkify">Date and time the record was last updated.</span></div>

</td>

<td class="column-type">

<div><span aria-hidden="true" class="icon icon-date"></span><span class="type-name" data-name="calendar_date">Date & Time</span></div>

</td>



</tr>


<tr class="column-summary" data-column="latitude" aria-expanded="false" aria-haspopup="true" role="link" tabindex="0">

<td class="column-name" scope="row">Latitude</td>

<td class="column-description">

<div class="contents clamped" data-original-height="21" style="height: 100px;"><span class="Linkify">The latitude of the location where the incident occurred. This location is shifted from the actual location for partial redaction but falls on the same block.</span></div>

</td>

<td class="column-type">

<div><span aria-hidden="true" class="icon icon-number"></span><span class="type-name" data-name="number">Number</span></div>

</td>



</tr>


<tr class="column-summary" data-column="longitude" aria-expanded="false" aria-haspopup="true" role="link" tabindex="0">

<td class="column-name" scope="row">Longitude</td>

<td class="column-description">

<div class="contents clamped" data-original-height="21" style="height: 100px;"><span class="Linkify">The longitude of the location where the incident occurred. This location is shifted from the actual location for partial redaction but falls on the same block.</span></div>

</td>

<td class="column-type">

<div><span aria-hidden="true" class="icon icon-number"></span><span class="type-name" data-name="number">Number</span></div>

</td>



</tr>



<tr class="column-summary" data-column="location" aria-expanded="false" aria-haspopup="true" role="link" tabindex="0">

<td class="column-name" scope="row">Location</td>

<td class="column-description">

<div class="contents clamped" data-original-height="21" style="height: 100px;"><span class="Linkify">The location where the incident occurred in a format that allows for creation of maps and other geographic operations on this data portal. This location is shifted from the actual location for partial redaction but falls on the same block.</span></div>

</td>

<td class="column-type">

<div><span aria-hidden="true" class="icon icon-map"></span><span class="type-name" data-name="location">Location</span></div>

</td>


</tr>

</tbody>

</table>











## Source of dataset:
[Chicago Crime Data from 2001 to present](https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-present/ijzp-q8t2)

## License

See the [LICENSE](https://github.com/k-chuang/chicago-crime-data-analysis/blob/master/LICENSE) file for license rights and limitations (MIT).


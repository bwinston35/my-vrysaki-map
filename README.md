# Template for Exploring Spatial Data and Building Interactive Maps

This template is a foundation for teaching others about spatial data, file types, and interactive mapping. After teaching about this in various settings, I decided to create a broader template that builds off of [Hands on DataViz](https://handsondataviz.org/). You can learn more about the original template below. If you are looking for more in-depth curriculum about version control, data wrangling, coding templates, web publishing, and more see the [Digital Scholarship Foundations Digital Mapping workshop series](https://puldischo.github.io/dsf-spring-2026/) I created as part of [Digital Scholarship Services](https://library.princeton.edu/services/digital-scholarship) at Princeton University Library.

## About the Data in this Template

The data is generated from objects from the [Messinesi Photographs Collection](https://collections.visualresources.princeton.edu/Detail/collections/SR-000072) which is part of the [Homer A. Thompson Collection](https://collections.visualresources.princeton.edu/Detail/collections/C-000008) house in [Visual Resources Collections](https://collections.visualresources.princeton.edu/) of Princeton University's Department of Art and Archaeology.

After georeferencing the map in the Messinesi Photographs Collection, I used Google Earth to geolocate each red marker on the map. The red markers represent a photograph in the collection. I then transformed the resulting `google-earth-points.kml` file into `google-earth-points.geojson` and `google-earth-points.csv` using the platform [geojson.io](https://geojson.io/). While the Google Earth-generated kml file has additional data that may not be necessary for your mapping needs, especially after transformed into csv format, it is still a great way to explore spatial data and compare different file types.

The `data.csv` file combines metadata from the Messinesi Photographs Collections and the extracted latitude and longitude coordinates from the `google-earth-points.kml` file to complete the dataset in order to allow users to build a map. If you follow along with the [Digital Scholarship Foundations Digital Mapping workshop series](https://puldischo.github.io/dsf-spring-2026/) your map will create a pop-up with some descriptive metadata and a photograph from the collection for each marker.

# leaflet-map-csv
Below is the information from [Hands on DataViz](https://handsondataviz.org/) on how to use the original tutorial that this repo is forked from.

## Demo
https://handsondataviz.github.io/leaflet-map-csv/

Sample data of select universities and colleges around CT by HandsOnDataViz.

## Make your own

1. Press **Use this template** button to create a copy of this repository in your own GitHub account.
2. Put your point data data inside `data.csv`. The only relevant columns that will be read by the template
are `Latitude`, `Longitude`, and `Title` (displayed in a popup). Sample data:
```
Title,Latitude,Longitude
Trinity College,41.745167,-72.69263
Wesleyan University,41.55709,-72.65691
```

For more information on customization, see [Leaflet documentation](https://leafletjs.com/).

## HandsOnDataViz Tutorial
https://handsondataviz.org/leaflet-maps-with-csv.html

## See other Leaflet templates
* [Simple Leaflet map](https://github.com/HandsOnDataViz/leaflet-map-simple)
* [Leaflet map with open data APIs](https://github.com/HandsOnDataViz/leaflet-maps-open-data-apis)
* [Leaflet map with data from Socrata](https://github.com/HandsOnDataViz/leaflet-socrata)
* [Leaflet polygon map with tabs](https://github.com/HandsOnDataViz/leaflet-map-polygon-tabs)
* [Leaflet heatmap](https://github.com/HandsOnDataViz/leaflet-heatmap)
* [Searcheable Map Template](https://github.com/HandsOnDataViz/searchable-map-template-csv)
* [Leaflet Maps with Google Sheets](https://github.com/HandsOnDataViz/leaflet-maps-with-google-sheets)
* [Leaflet Storymaps with Google Sheets](https://github.com/HandsOnDataViz/leaflet-storymaps-with-google-sheets)

## DOB NOW: Build Milestones

The New York City Department of Buildings (DOB) DOB NOW Build Milestones application displays basic details for selected DOB NOW Build filings on an interactive map of New York City. Each filing is represented as a dot on the map, and clicking the dot or the item on the list below brings you to a profile page that shows major milestone dates for that filing. The application is updated daily with the latest filings for Antenna, Curb Cut, Fence, Plumbing, Scaffold, Sidewalk Shed, Sign, Sprinkler, and Standpipe filings in DOB NOW.

![Milestone Map Page](https://github.com/cnicklin/D3_DOBNOW_Milestone/blob/gh-pages/MapPage.PNG)

## Data Source

Data flows from the BI tool to GitHub public hold. This is a daily automated process. It creates results in 2 formats: JSON (for search) and CSV (for map imaging).

<img align="center" width="" height="" src="https://github.com/cnicklin/D3_DOBNOW_Milestone/blob/gh-pages/Flow.PNG" alt="Milestone App Flow Diagram">

## Data Definitions
A definition for each of the values for Filing Status can be found on our [Status Glossary](https://github.com/cnicklin/D3_DOBNOW_Milestone/blob/gh-pages/Statuses.md).

Definitions for elements on the Profile Page are listed below, but can also be viewed by hovering over the field name on the webpage.

### Profile Page

| Metric | Definition |
|-------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Borough | Indicates which of the 5 NYC boroughs the building is located in |
| Year Built | Indicates the year that the building was built (source: NYC Building Footprints) |
| BIN Profile | Provides a link to the building’s profile page on Building Information System (BIS), where you can find more detail about every transaction that the building has with DOB |
| Cyclomedia Street View | A photo of the building taken from the street by [Cyclomedia](https://www.cyclomedia.com/us). This may or may not show active construction work that corresponds with what is reported in the data |
| 12-month building statistics | This section shows the count of all permits, complaints, inspections, violations, and accidents in the past 12 months from today that correspond to this building |


## Built With

* [R](https://www.r-project.org/)
    + Core packages(dplyr, tidyr, RJDBC, ...)
* [Carto VL](https://carto.com/developers/carto-vl/)
* [Mapbox GL](https://www.mapbox.com/mapbox-gl-js/api/)
* [D3](https://d3js.org/)
* [Bootstrap](https://getbootstrap.com/)

## Built by

* [DOB Analytics and Data Science Team](https://www1.nyc.gov/site/buildings/about/metrics-reports.page) - If you have questions or feedback, comment here on github or email us at [Analytics@buildings.nyc.gov](mailto:analytics@buildings.nyc.gov). (Note: We're hiring a web developer!)

## Acknowledgments

* Inspired by [NYC Planning Labs](https://planninglabs.nyc/)


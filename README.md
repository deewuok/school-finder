# OKC School Finder

Geolocation-based web app for locating schools and school districts near you.


### Phase 1
* Frontend
  * [ ] Single page site
  * [ ] Landing page
  * [ ] Reverse geocode address into lat lon location
  * [ ] Show school district for a given lat lon location
  * [ ] Show closest schools to a given lat lon location (restricted by school district?)
* Data/backend
  * [ ] Static JSON dataset for school districts and schools suitable for identifying school districts and schools via distance calculations
  * [ ] Tools for generating dataset(s)
* Deployment
  * [ ] Hosting of site and data (s3?)
  * [ ] Automated data update/ingest (?)

### Phase 2
TBD

## Technical Details

### Data Upload/Translate Process

* *Ongoing discussion: https://github.com/codeforokc/school-finder/issues/4*

### Client

* Create [Mapbox](https://www.mapbox.com/) map without dataset
* Use [Turf](http://turfjs.org/) to query for distance information
* Use [Leaflet](http://leafletjs.com/) or [Turf](http://turfjs.org/) to query for polygon information at a point
* Use [Leaflet](http://leafletjs.com/) to visualize schools/school districts on top of Mapbox map via dataset
* Use [Mapbox Geocoding API](https://www.mapbox.com/developers/api/geocoding/) for reverse geocoding addresses

## Data

* [School District Boundaries](http://data.okc.gov/applications/datadownload/forms/DownloadDetails.aspx?DataSetID=3) via data.okc.gov
* [Schools](http://data.okc.gov/applications/datadownload/forms/DownloadDetails.aspx?DataSetID=17) via data.okc.gov

## Contributing

If you would like to contribute code, just fork the repository and work on a new branch. You can submit a pull request to our repository and a member of Code for OKC will approve and merge it.

## Copyright and license

Copyright 2014 Code for OKC. Licensed under the MIT License.

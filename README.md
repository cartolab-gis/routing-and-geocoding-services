# Routing and Geocoding: APIs and Engines

## SUMMARY

This document contains a review of the current state of Routing and Geocoding APIs and engines. It covers multiple options, ranging from free & open source options that can be self-hosted to paid services.

In this document:

_Routing_ refers to a set of several different functionalities, such as:

* Point-to-Point Routing/Directions

* Route Optimization

* Distance Matrix

* Isochrones/Drive Time Areas

* Turn-by-Turn Navigation

_Geocoding_ refers to a set of tools such as:

* Single Address Search

* Batch Geocoding

* Reverse Geocoding

* POI Search

Routing and Geocoding are two geospatial processes that are often requirements for web applications.

### Services Covered

* ArcGIS Online

* Mapbox

* CARTO

* Google

* Bing

* Mapquest

* HERE

* OpenRouteService

* GraphHopper

* OpenCageData

* LocationIQ

* Valhalla

* Pelias

* OSRM

* pgRouting

# ARCGIS ONLINE

ArcGIS Online (AGO) is a cloud-based service from ESRI. It’s a full geospatial platform, not just Routing and Geocoding. This analysis just focuses on Routing and Geocoding services.

Details on Routing/Directions Services: [https://developers.arcgis.com/features/directions/](https://developers.arcgis.com/features/directions/)

Details on Geocoding: [https://developers.arcgis.com/features/geocoding/](https://developers.arcgis.com/features/geocoding/)

<table>
  <tr>
    <td>Services Available</td>
    <td>Routing

* [x] Point-to-Point Routing/Directions
* [x] Route Optimization
* [x] Distance Matrix
* [x] Isochrones/Drive Time Areas
* [ ] Snap To Roads
* [x] Traffic Data/Integration
* [ ] Public Transit

      </td>

    <td>Geocoding

  * [x] Single Address Search
  * [x] Batch Geocoding
  * [x] Reverse Geocoding
  * [x] POI Search
  * [x] Autocomplete

        </td>

          </tr>

        <tr>
        <td>License Terms</td>
        <td>Free tier available for public/non-commercial apps, restricted to displaying results on ESRI maps/products.  Paid plans for commercial that have no display restrictions and allow for saving results to a database.

    Full terms: https://developers.arcgis.com/terms/ </td>
    <td></td>

      </tr>
  <tr>
    <td>Pricing</td>
    <td>Contributor Seat: $504/year ($42/month).  Viewer seats are $9/month, but Viewers are meant to be within the organization, not ‘app users’.  ESRI wants you to manage app users separately.</td>
    <td></td>
  </tr>
</table>

# MAPBOX

MapBox offers a variety of data services and APIs, including driving directions/routing and geocoding.

<table>
  <tr>
    <td>Services Available</td>
    <td>Routing and Geocoding APIs (plus others)</td>
  </tr>
  <tr>
    <td>License Terms</td>
    <td>Free/Pay-as-you-go  tier available for public/non-commercial apps.  Commercial plans are required for any application that requires fees or has restricted access.</td>
  </tr>
  <tr>
    <td>Pricing</td>
    <td>Commercial plans start at $499/month</td>
  </tr>
</table>

# CARTO

CARTO is similar to ArcGIS Online in that it is a full geospatial platform. It offers two distinct products: Builder and Engine. The data APIs and services like routing and geocoding are part of the Engine plan, which is also need to build custom applications.

Note: Some of CARTO’s data services were powered by the now defunct Mapzen. It’s unclear what impact this change has on the future of CARTO’s data services.

<table>
  <tr>
    <td>Services Available</td>
    <td>Routing and Geocoding APIs (plus others)</td>
  </tr>
  <tr>
    <td>License Terms</td>
    <td></td>
  </tr>
  <tr>
    <td>Pricing</td>
    <td>Engine plans start at $9,900/year</td>
  </tr>
</table>

# GOOGLE

<table>
  <tr>
    <td>Services Available</td>
    <td>Routing and Geocoding APIs (plus others)</td>
  </tr>
  <tr>
    <td>License Terms</td>
    <td>Free/Pay-as-you-go tier available for public/non-commercial apps.  Commercial plans are required for any application that requires fees or has restricted access.</td>
  </tr>
  <tr>
    <td>Pricing</td>
    <td>Commercial plans start at $10,000/year</td>
  </tr>
</table>

# BING

Offers REST APIs.

<table>
  <tr>
    <td>Services Available</td>
    <td>Routing
Point-to-Point Routing/Directions
Route Optimization
Distance Matrix
Isochrones/Drive Time Areas
Snap To Roads
Traffic Data/Integration
Public Transit</td>
    <td>Geocoding
Single Address Search
Batch Geocoding*
Reverse Geocoding
POI Search*
Autocomplete
*with Spatial Data Services</td>
  </tr>
  <tr>
    <td>License Terms</td>
    <td>https://www.microsoft.com/en-us/maps/licensing/options
https://www.microsoft.com/en-us/maps/product 
Major Points:
Commercial/Internal Business apps with "limited usage" (under 125k billable transactions per year) may qualify for regular/free Bing accounts.
On free/basic accounts, Microsoft reserves right to include a search box and </td>
    <td></td>
  </tr>
  <tr>
    <td>Pricing</td>
    <td>
https://msdn.microsoft.com/en-us/library/ff859477.aspx</td>
    <td></td>
  </tr>
</table>

# MAPQUEST

<table>
  <tr>
    <td>Services Available</td>
    <td>Routing
Point-to-Point Routing/Directions
Route Optimization
Distance Matrix
Isochrones/Drive Time Areas
Snap To Roads
Traffic Data/Integration
Public Transit</td>
    <td>Geocoding
Single Address Search
Batch Geocoding
Reverse Geocoding
POI Search
Autocomplete
</td>
  </tr>
  <tr>
    <td>License Terms</td>
    <td>https://developer.mapquest.com/legal
Major Points:
Can use plans commercially (even free)
Can’t store results without enhanced plan
Results (at least geocodes) have to be displayed on a MapQuest map.</td>
    <td></td>
  </tr>
  <tr>
    <td>Pricing</td>
    <td>Several tiers, starting at Free:
https://developer.mapquest.com/plans
</td>
    <td></td>
  </tr>
</table>

# HERE

HERE is actually one of the oldest data providers in this list. Great set of APIs, some of which don’t exist in other services (e.g. weather, venues). .

<table>
  <tr>
    <td>Services Available</td>
    <td>Routing
Point-to-Point Routing/Directions
Route Optimization
Distance Matrix
Isochrones/Drive Time Areas
Snap To Roads
Traffic Data/Integration
Public Transit</td>
    <td>Geocoding
Single Address Search
Batch Geocoding
Reverse Geocoding
POI Search
Autocomplete
</td>
  </tr>
  <tr>
    <td>License Terms</td>
    <td>Tiers split depending on intended usage:
Major Points
Can display results on Leaflet of Openlayers but not on maps from competing services (e.g. Google, Mapbox, ESRI?) </td>
    <td></td>
  </tr>
  <tr>
    <td>Pricing</td>
    <td>https://developer.here.com/plans

Commercial Apps start at $199/mo (discount for yearly payment)

</td>
    <td></td>
  </tr>
</table>

# GRAPHHOPPER

<table>
  <tr>
    <td>Services Available</td>
    <td>Routing and Geocoding APIs (plus others)</td>
  </tr>
  <tr>
    <td>License Terms</td>
    <td>https://www.graphhopper.com/terms/ 
Major Points:
Generally very lenient terms.  Commercial usage allowed on all but free plans.  Can use Directions APIs for navigation.</td>
  </tr>
  <tr>
    <td>Pricing</td>
    <td>https://www.graphhopper.com/pricing/
Pay attention to how many credits requests consume.  Things like Isochrones are relatively limited/expensive.
</td>
  </tr>
  <tr>
    <td>Self-Hosted Requirements</td>
    <td>The GraphHopper OS project can be self-hosted:
https://www.graphhopper.com/open-source/
Deployment Guide:
https://github.com/graphhopper/graphhopper/blob/master/docs/core/deploy.md 
A planet-sized OSM extract needs 22GB RAM to preprocess and then 15GB RAM to run.  North America (easier to download directly than a US-specific extract) would be a little under ¼ the requirements.
North America extract: 
preprocessing - 5 GB RAM
running: 4GB RAM
Probably need about 20-30 GB of storage
DigitalOcean: A North American extract could potentially run on a High-Memory Digital Ocean instance for $40-60/month
AWS:
Somewhere between $60-100/month 
https://calculator.s3.amazonaws.com/index.html#r=IAD&s=EC2&key=calc-6453E001-6882-4F10-BF6D-9FB56F967DCE
Differences in hosted and open source projects:
</td>
  </tr>
</table>

# OSRM

<table>
  <tr>
    <td>Services Available</td>
    <td>Routing only
Point-to-Point Routing/Directions
Route Optimization
Distance Matrix
Isochrones/Drive Time Areas
Snap To Roads
Traffic Data/Integration
Public Transit</td>
  </tr>
  <tr>
    <td>License Terms</td>
    <td>Open source. BSD License</td>
  </tr>
  <tr>
    <td>Self-Hosted Requirements</td>
    <td>https://github.com/Project-OSRM/osrm-backend/wiki/Disk-and-Memory-Requirements 
OSM Planet: 
Car-only preprocessing 175 GB RAM, 280GB Disk Space for STXXL, ~80GB Storage for files
Car runtime: 64GB RAM + 50GB Storage for preprocessed files
North America:
preprocessing: 40GB RAM, 80-100GB Storage
Runtime: 14GB RAM, 12-20GB Storage</td>
  </tr>
</table>

# PELIAS

<table>
  <tr>
    <td>Services Available</td>
    <td>Geocoding/Search Engine</td>
  </tr>
  <tr>
    <td>License Terms</td>
    <td></td>
  </tr>
  <tr>
    <td>Self-Hosted Requirements</td>
    <td></td>
  </tr>
</table>

# VALHALLA

<table>
  <tr>
    <td>Services Available</td>
    <td>Geocoding/Search Engine</td>
  </tr>
  <tr>
    <td>License Terms</td>
    <td></td>
  </tr>
  <tr>
    <td>Self-Hosted Requirements</td>
    <td></td>
  </tr>
</table>

# OPEN CAGE DATA

A dedicated geocoding API with generous free tier.

<table>
  <tr>
    <td>Services Available</td>
    <td>Geocoding
Single Address Search
Batch Geocoding
Reverse Geocoding
POI Search
Autocomplete</td>
  </tr>
  <tr>
    <td>License Terms</td>
    <td>Generous licensing terms, no restrictions on commercial use other than they ask to use a paid plan for any production deployments. </td>
  </tr>
  <tr>
    <td>Pricing</td>
    <td>https://geocoder.opencagedata.com/pricing
Monthly:

Yearly:

</td>
  </tr>
</table>

# LOCATION IQ

<table>
  <tr>
    <td>Services Available</td>
    <td>Geocoding
Single Address Search
Batch Geocoding
Reverse Geocoding
POI Search
Autocomplete</td>
  </tr>
  <tr>
    <td>License Terms</td>
    <td>Can’t use free tier for commercial applications</td>
  </tr>
  <tr>
    <td>Pricing</td>
    <td>https://locationiq.org/#pricing
</td>
  </tr>
</table>

# OPENROUTESERVICE

[https://go.openrouteservice.org/](https://go.openrouteservice.org/)

Notes: Geocoding/Addressing using OSM only (similar to Nominatim) and may not be good enough for commercial applications.

<table>
  <tr>
    <td>Services Available</td>
    <td>Routing & Geocoding APIs (plus others)</td>
  </tr>
  <tr>
    <td>License Terms</td>
    <td>Free to use for up to 2500 requests per day (including commercial use).</td>
  </tr>
  <tr>
    <td>Pricing</td>
    <td>https://go.openrouteservice.org/plans/
Free with rate limits.  Custom self-hosted installations available, with support.  Contact for pricing info.</td>
  </tr>
</table>

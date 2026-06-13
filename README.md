# 🐾 香港寵物食店牌照地圖 · Hong Kong Pet Food Shop Licences

An interactive map of licensed pet food shops in Hong Kong, with a district filter and search.

**Live map:** https://lau1991.github.io/hk-pet-food-map/

## Features
- Individual pin per shop, clustered by area, click for details (name, address, licence no., Google Maps link)
- Filter by Hong Kong district; search by shop name or address
- Two-way link between the list and the map
- Accuracy tiers: **building-level** (blue) via the HK Lands Department address service, **street-level** (amber), and **district-centre approx** (red)

## Data & geocoding
- Source: pet food shop licence list (1,000 shops)
- Coordinates resolved via the HK government LocationSearch API (`www.map.gov.hk`), converted from HK1980 Grid to WGS84 (inverse Transverse Mercator + 7-parameter Helmert)

## Tech
Single static `index.html` — [Leaflet](https://leafletjs.com/) + MarkerCluster, CARTO Voyager basemap. No build step.

# Power BI Custom Map Visual

This project is a custom visual for Power BI that renders interactive maps using vector tiles, clustered point data, and custom HTML elements. The visual is built with Leaflet and integrates with a custom API that serves vector tiles from an external tile server.

## Features

- Multiple map types: vector tiles, clustering, and custom UI controls
- Uses Leaflet for rendering and OpenStreetMap as a base map
- API layer for fetching vector tiles securely and efficiently
- Supports high-density spatial data and dynamic zoom behavior

## Project structure

This visual is split into multiple `visual.ts` implementations, each with its own use case:

### Vector tile map

- Displays area-based data using vector tile layers.
- Vector tiles are fetched from API.
- Suitable for visualizing regions, boundaries, and other polygonal data.

### Clustered map

- Displays large point datasets using the `supercluster` library.
- Automatically clusters and updates dynamically based on zoom level.
- Great for performance and clarity with high data volume.

### HTML Controls on map

- Adds custom HTML UI elements (e.g. zoom in/out buttons) on top of the map.
- Positioned using Leaflet's control structures.
- Fully styleable via CSS.

## API

The custom visual retrieves vector tiles via a dedicated API that acts as a proxy to an external vector tile server.

## Technologies used

* Leaflet.js
* OpenStreetMap
* Supercluster
* Power BI Custom Visual SDK
* Vector tiles (.pbf)
* Node.js

## Project Limitations
Due to the proprietary nature of the code used in the project, I cannot share the source code.

<h1>Utility Emergency Response Routing & Service Coverage Analysis</h1>

<h2>Operational GIS Network Analysis Using Open-Source Geospatial Tools</h2>

<p>
  <img src="outputs/screenshots/emergency_response_routes.png" alt="Utility Emergency Response Routing Analysis" width="100%">
</p>

<hr>

<h2>Project Overview</h2>

<p>
Utility organizations need efficient ways to evaluate how emergency response crews can reach outage events, infrastructure failures, and service disruption locations across a transportation network.
</p>

<p>
This project simulates a utility emergency response workflow in Washington, DC using open-source geospatial tools, transportation-network analysis, spatial SQL, and interactive web GIS visualization.
</p>

<p>
The main goal is to evaluate how utility response crews may travel from operational depots to simulated outage events using road-network routing analysis. The project also evaluates service coverage, outage accessibility, affected transportation infrastructure, and operational response patterns.
</p>

<p>
This project is designed as a geospatial engineering portfolio case study, not just a static map. It combines Python-based GIS automation, network analysis, portable spatial storage, spatial SQL analytics, QGIS validation, and browser-based web mapping.
</p>

<hr>

<h2>Operational Problem</h2>

<p>
During outage events, utility operators need to answer practical spatial questions:
</p>

<ul>
  <li>Which utility depot should respond to each outage?</li>
  <li>What is the shortest transportation-network route?</li>
  <li>Which outage events are outside approximate service coverage?</li>
  <li>Which road segments are near outage impact zones?</li>
  <li>Where are potential emergency response accessibility gaps?</li>
</ul>

<hr>

<h2>Key Skills Demonstrated</h2>

<ul>
  <li>Transportation network acquisition with OSMnx</li>
  <li>Shortest-path routing with NetworkX</li>
  <li>GeoPandas vector spatial analysis</li>
  <li>CRS-aware spatial processing</li>
  <li>Utility depot and outage event simulation</li>
  <li>Service coverage analysis</li>
  <li>Infrastructure impact buffer analysis</li>
  <li>Spatial overlay analysis</li>
  <li>GeoPackage spatial storage</li>
  <li>DuckDB Spatial SQL querying</li>
  <li>QGIS validation and cartographic preparation</li>
  <li>GeoJSON export for web GIS</li>
  <li>Leaflet interactive web mapping</li>
</ul>

<hr>

<h2>Project Workflow</h2>

<pre>
OpenStreetMap Road Network
        ↓
OSMnx Network Acquisition
        ↓
NetworkX Shortest-Path Routing
        ↓
GeoPandas Spatial Processing
        ↓
Service Coverage and Infrastructure Impact Analysis
        ↓
GeoPackage Spatial Storage
        ↓
DuckDB Spatial SQL Analytics
        ↓
QGIS Validation and Cartographic Review
        ↓
GeoJSON Export
        ↓
Leaflet Interactive Web GIS
</pre>

<hr>

<h2>Technology Stack</h2>

<table>
  <tr><th>Component</th><th>Technology</th></tr>
  <tr><td>Desktop GIS</td><td>QGIS</td></tr>
  <tr><td>Spatial Analysis</td><td>Python, GeoPandas, Shapely</td></tr>
  <tr><td>Transportation Network</td><td>OSMnx, OpenStreetMap</td></tr>
  <tr><td>Routing Engine</td><td>NetworkX</td></tr>
  <tr><td>Spatial SQL</td><td>DuckDB Spatial</td></tr>
  <tr><td>Spatial Storage</td><td>GeoPackage</td></tr>
  <tr><td>Web GIS</td><td>Leaflet, GeoJSON</td></tr>
  <tr><td>Notebook Environment</td><td>JupyterLab</td></tr>
</table>

<hr>

<h2>Data Sources</h2>

<h3>Transportation Network</h3>

<p>
The drivable road network was downloaded from OpenStreetMap using OSMnx.
</p>

<ul>
  <li>Source: OpenStreetMap</li>
  <li>Access Method: OSMnx Python library</li>
  <li>Network Type: Drivable road network</li>
  <li>Study Area: Washington, District of Columbia, USA</li>
</ul>

<h3>Utility Depots and Outage Events</h3>

<p>
Utility depot locations and outage events are simulated for analytical demonstration purposes. They are not real utility assets or real outage incidents.
</p>

<hr>

<h2>Project Structure</h2>

<pre>
Utility Emergency Response Routing/
│
├── data/
│   └── processed/
│       ├── roads.gpkg
│       ├── utility_depots.gpkg
│       └── utility_emergency_response_routing.gpkg
│
├── notebooks/
│   └── utility_emergency_routing_analysis.ipynb
│
├── webmap/
│   ├── index.html
│   └── data/
│       ├── roads.geojson
│       ├── utility_depots.geojson
│       ├── utility_outages.geojson
│       ├── emergency_response_routes.geojson
│       └── utility_service_areas.geojson
│
├── outputs/
│   └── screenshots/
│       ├── transportation_road_network.png
│       ├── utility_depot_locations.png
│       ├── depot_and_outage_locations.png
│       ├── emergency_response_routes.png
│       ├── service_coverage_analysis.png
│       ├── infrastructure_impact_analysis.png
│       └── leaflet_webmap.png.png
│
├── README.md
├── requirements.txt
└── .gitignore
</pre>

<hr>

<h2>Analysis Summary</h2>

<h3>1. Transportation Network Acquisition</h3>

<p>
The project begins by downloading the Washington, DC drivable road network using OSMnx. The network is converted into GeoDataFrames representing road segments and network nodes.
</p>

<p>
  <img src="outputs/screenshots/transportation_road_network.png" alt="Washington DC Transportation Road Network" width="100%">
</p>

<h3>2. Utility Depot Simulation</h3>

<p>
Simulated utility depot locations are created as operational response origins. These depots represent where crews or maintenance vehicles may be dispatched during emergency events.
</p>

<p>
  <img src="outputs/screenshots/utility_depot_locations.png" alt="Simulated Utility Emergency Response Depots" width="100%">
</p>

<h3>3. Outage Event Simulation</h3>

<p>
Simulated outage events are created across Washington, DC. Each outage includes an outage ID, priority level, affected customer estimate, and point geometry.
</p>

<p>
  <img src="outputs/screenshots/depot_and_outage_locations.png" alt="Utility Depot and Outage Locations" width="100%">
</p>

<h3>4. Emergency Routing Analysis</h3>

<p>
The workflow uses NetworkX to calculate shortest-path routes between utility depots and outage events across the OpenStreetMap road network.
</p>

<p>
Each outage is assigned to the depot with the shortest network-based route.
</p>

<p>
  <img src="outputs/screenshots/emergency_response_routes.png" alt="Utility Emergency Response Routing Analysis" width="100%">
</p>

<h3>5. Service Coverage Analysis</h3>

<p>
Approximate service coverage zones are generated around utility depots to evaluate response accessibility and potential coverage gaps.
</p>

<p>
  <img src="outputs/screenshots/service_coverage_analysis.png" alt="Utility Emergency Response Service Coverage" width="100%">
</p>

<h3>6. Infrastructure Impact Analysis</h3>

<p>
Outage impact zones are generated around outage events, and nearby road segments are identified using spatial overlay analysis.
</p>

<p>
  <img src="outputs/screenshots/infrastructure_impact_analysis.png" alt="Transportation Infrastructure Near Outage Events" width="100%">
</p>

<h3>7. Spatial SQL Analysis</h3>

<p>
The project uses DuckDB Spatial to query GeoPackage layers directly using SQL. This provides a lightweight alternative to a full PostGIS server while preserving spatial SQL capabilities.
</p>

<pre>
SELECT
    outage_id,
    assigned_depot,
    ROUND(route_distance_meters / 1000.0, 2) AS route_distance_km
FROM emergency_response_routes
ORDER BY route_distance_km DESC;
</pre>

<h3>8. Interactive Web GIS</h3>

<p>
Final operational layers are exported to GeoJSON and displayed in an interactive Leaflet web map.
</p>

<p>
  <img src="outputs/screenshots/leaflet_webmap.png.png" alt="Leaflet Interactive Web Map" width="100%">
</p>

<hr>

<h2>Interactive Web Map</h2>

<p>
The interactive Leaflet map is stored at:
</p>

<pre>
webmap/index.html
</pre>

<p>
To run it locally:
</p>

<pre>
cd webmap
python3 -m http.server 8000
</pre>

<p>
Then open:
</p>

<pre>
http://localhost:8000
</pre>

<hr>

<h2>QGIS Workflow</h2>

<p>
QGIS is used as a desktop GIS validation and cartographic production environment.
</p>

<p>
The QGIS workflow supports:
</p>

<ul>
  <li>reviewing GeoPackage layers</li>
  <li>validating CRS alignment</li>
  <li>inspecting road network coverage</li>
  <li>checking route geometry</li>
  <li>reviewing depot and outage placement</li>
  <li>styling operational layers</li>
  <li>creating a professional map layout</li>
</ul>

<p>
Recommended QGIS input:
</p>

<pre>
data/processed/utility_emergency_response_routing.gpkg
</pre>

<hr>

<h2>Technical Notes</h2>

<h3>CRS Strategy</h3>

<p>
The workflow uses EPSG:26918, NAD83 / UTM Zone 18N, for distance-based GIS analysis in the Washington, DC region.
</p>

<p>
Layers are converted back to EPSG:4326 for GeoJSON export and Leaflet web mapping.
</p>

<h3>Routing Method</h3>

<p>
Emergency response routes are calculated using shortest-path routing on the drivable road network. This provides a realistic improvement over straight-line distance analysis because movement follows transportation infrastructure.
</p>

<h3>Spatial Storage Strategy</h3>

<p>
The project originally considered PostGIS for spatial database integration. The workflow was redesigned to use GeoPackage and DuckDB Spatial to improve portability, reduce setup complexity, and make the project easier to reproduce from GitHub.
</p>

<h3>Service Coverage Modeling</h3>

<p>
Service coverage areas are modeled using simplified buffer-based zones around utility depots. This provides an interpretable first-stage view of operational coverage but does not replace true network-based service areas.
</p>

<hr>

<h2>Results and Operational Insights</h2>

<ul>
  <li>The workflow successfully models emergency response routing from simulated utility depots to outage events.</li>
  <li>Network-based routes provide more realistic accessibility patterns than straight-line distance.</li>
  <li>Service coverage zones reveal that not all outage locations fall within approximate response coverage.</li>
  <li>Spatial SQL analysis supports route-distance review and outage accessibility interpretation.</li>
  <li>Infrastructure impact zones highlight road segments near outage locations that may affect emergency response operations.</li>
</ul>

<hr>

<h2>Limitations</h2>

<ul>
  <li>Utility depot and outage locations are simulated.</li>
  <li>Routes use network distance rather than live travel time.</li>
  <li>Traffic conditions are not modeled.</li>
  <li>Road restrictions and vehicle-specific routing constraints are not included.</li>
  <li>Service coverage uses Euclidean buffers rather than network-based service areas.</li>
  <li>OpenStreetMap data quality may vary by location.</li>
  <li>The project is intended as a GIS engineering demonstration, not an operational utility system.</li>
</ul>

<hr>

<h2>Future Improvements</h2>

<ul>
  <li>Implement travel-time-based routing.</li>
  <li>Add network-based service area generation.</li>
  <li>Integrate traffic speed assumptions.</li>
  <li>Add road closure or blocked-route simulation.</li>
  <li>Include real utility assets if public data is available.</li>
  <li>Add outage severity scoring.</li>
  <li>Improve QGIS cartographic layout and labeling.</li>
  <li>Deploy the Leaflet web map using GitHub Pages.</li>
  <li>Add reusable Python scripts outside the notebook.</li>
  <li>Package routing and coverage logic into a small Python toolkit.</li>
</ul>

<hr>

<h2>How to Run the Project</h2>

<h3>1. Clone the Repository</h3>

<pre>
git clone git@github.com:namozhdehi/utility-emergency-response-routing-analysis.git
cd utility-emergency-response-routing-analysis
</pre>

<h3>2. Create and Activate a Virtual Environment</h3>

<pre>
python3 -m venv .venv
source .venv/bin/activate
</pre>

<h3>3. Install Dependencies</h3>

<pre>
pip install -r requirements.txt
</pre>

<h3>4. Launch JupyterLab</h3>

<pre>
jupyter lab
</pre>

<h3>5. Open the Notebook</h3>

<pre>
notebooks/utility_emergency_routing_analysis.ipynb
</pre>

<h3>6. Run the Web Map Locally</h3>

<pre>
cd webmap
python3 -m http.server 8000
</pre>

<p>
Then open:
</p>

<pre>
http://localhost:8000
</pre>

<hr>

<h2>Repository Notes</h2>

<p>
The repository includes small processed GIS outputs required for reproducibility and web mapping.
</p>

<p>
The following local files and folders are intentionally excluded from GitHub:
</p>

<pre>
.venv/
cache/
.ipynb_checkpoints/
.DS_Store
__pycache__/
</pre>

<hr>

<h2>Author</h2>

<p>
<strong>Nahid Mozhdehi</strong>
</p>

<p>
GIS and geospatial engineering portfolio project focused on open-source GIS, network analysis, spatial SQL, and operational web mapping.
</p>

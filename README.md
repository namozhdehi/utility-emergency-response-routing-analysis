<h1>Utility Emergency Response Routing & Service Coverage Analysis</h1>

<h2>Operational GIS Network Analysis Using Open-Source Geospatial Tools</h2>

<p>
  <img src="outputs/screenshots/leaflet_webmap_full_interface.png" alt="Utility Emergency Response Web GIS" width="100%">
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
The workflow models how utility crews may travel from operational depots to outage events using network-based routing analysis across the OpenStreetMap transportation network.
</p>

<p>
The project combines:
</p>

<ul>
  <li>Python-based GIS automation</li>
  <li>Transportation network analysis</li>
  <li>GeoPandas spatial processing</li>
  <li>Spatial SQL analytics</li>
  <li>DuckDB Spatial integration</li>
  <li>QGIS validation workflows</li>
  <li>Leaflet interactive web mapping</li>
</ul>

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

<p>
This project models those operational questions through a reproducible open-source GIS workflow.
</p>

<hr>

<h2>Key Skills Demonstrated</h2>

<ul>
  <li>Transportation network acquisition with OSMnx</li>
  <li>Shortest-path routing with NetworkX</li>
  <li>GeoPandas vector spatial analysis</li>
  <li>CRS-aware spatial processing</li>
  <li>Utility depot and outage simulation</li>
  <li>Infrastructure impact analysis</li>
  <li>Service coverage analysis</li>
  <li>GeoPackage spatial storage</li>
  <li>DuckDB Spatial SQL querying</li>
  <li>QGIS validation and cartography</li>
  <li>GeoJSON export workflows</li>
  <li>Leaflet web GIS development</li>
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
Service Coverage Analysis
        ↓
Infrastructure Impact Analysis
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
  <tr>
    <th>Component</th>
    <th>Technology</th>
  </tr>

  <tr>
    <td>Desktop GIS</td>
    <td>QGIS</td>
  </tr>

  <tr>
    <td>Spatial Analysis</td>
    <td>Python, GeoPandas, Shapely</td>
  </tr>

  <tr>
    <td>Transportation Network</td>
    <td>OSMnx, OpenStreetMap</td>
  </tr>

  <tr>
    <td>Routing Engine</td>
    <td>NetworkX</td>
  </tr>

  <tr>
    <td>Spatial SQL</td>
    <td>DuckDB Spatial</td>
  </tr>

  <tr>
    <td>Spatial Storage</td>
    <td>GeoPackage</td>
  </tr>

  <tr>
    <td>Web GIS</td>
    <td>Leaflet, GeoJSON</td>
  </tr>

  <tr>
    <td>Notebook Environment</td>
    <td>JupyterLab</td>
  </tr>
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
├── outputs/
│   └── screenshots/
│       ├── transportation_road_network.png
│       ├── utility_depot_locations.png
│       ├── depot_and_outage_locations.png
│       ├── emergency_response_routes.png
│       ├── service_coverage_analysis.png
│       ├── infrastructure_impact_analysis.png
│       ├── leaflet_webmap_clean.png
│       ├── leaflet_webmap_full_interface.png
│       └── final_operational_qgis_layout.png
│
├── webmap/
│   ├── index.html
│   └── data/
│
├── requirements.txt
├── README.md
└── .gitignore
</pre>

<hr>

<h2>Analysis Summary</h2>

<h3>1. Transportation Network Acquisition</h3>

<p>
The workflow begins by downloading the Washington, DC drivable transportation network using OSMnx.
</p>

<p>
The road network provides the routing foundation for all emergency response analysis.
</p>

<p>
  <img src="outputs/screenshots/transportation_road_network.png" alt="Washington DC Transportation Road Network" width="80%">
</p>

<hr>

<h3>2. Utility Depot Simulation</h3>

<p>
Simulated utility depots are generated as operational response origins for emergency routing analysis.
</p>

<p>
These depots represent possible utility dispatch centers across Washington, DC.
</p>

<p>
  <img src="outputs/screenshots/utility_depot_locations.png" alt="Utility Depot Locations" width="80%">
</p>

<hr>

<h3>3. Outage Event Simulation</h3>

<p>
Simulated outage events are distributed across the transportation network to model emergency response scenarios.
</p>

<p>
Each outage includes simulated operational attributes such as priority level and affected infrastructure.
</p>

<p>
  <img src="outputs/screenshots/depot_and_outage_locations.png" alt="Utility Depot and Outage Locations" width="80%">
</p>

<hr>

<h3>4. Emergency Routing Analysis</h3>

<p>
NetworkX shortest-path routing is used to calculate transportation-network routes between utility depots and outage events.
</p>

<p>
The routing workflow models how utility response crews may travel through the road network instead of relying on unrealistic straight-line distance analysis.
</p>

<p>
  <img src="outputs/screenshots/emergency_response_routes.png" alt="Emergency Response Routing Analysis" width="80%">
</p>

<hr>

<h3>5. Service Coverage Analysis</h3>

<p>
Approximate utility service coverage zones are generated around operational depots.
</p>

<p>
This analysis helps identify outage locations that may fall outside estimated emergency response coverage.
</p>

<p>
  <img src="outputs/screenshots/service_coverage_analysis.png" alt="Service Coverage Analysis" width="80%">
</p>

<hr>

<h3>6. Infrastructure Impact Analysis</h3>

<p>
Infrastructure impact zones are generated around outage events to identify nearby transportation segments potentially affected during emergency operations.
</p>

<p>
Spatial overlay analysis is used to identify roads intersecting outage impact areas.
</p>

<p>
  <img src="outputs/screenshots/infrastructure_impact_analysis.png" alt="Infrastructure Impact Analysis" width="80%">
</p>

<hr>

<h3>7. Spatial SQL Analytics</h3>

<p>
The workflow integrates DuckDB Spatial for lightweight spatial SQL analysis directly against GeoPackage layers.
</p>

<p>
DuckDB Spatial was selected instead of PostGIS to improve:
</p>

<ul>
  <li>project portability</li>
  <li>GitHub reproducibility</li>
  <li>local execution simplicity</li>
  <li>lightweight deployment</li>
</ul>

<p>
Example SQL query:
</p>

<pre>
SELECT
    outage_id,
    assigned_depot,
    ROUND(route_distance_meters / 1000.0, 2) AS route_distance_km
FROM emergency_response_routes
ORDER BY route_distance_km DESC;
</pre>

<hr>

<h3>8. Interactive Web GIS</h3>

<p>
Final operational layers are exported to GeoJSON and visualized through a Leaflet interactive web map.
</p>

<p>
The web map includes:
</p>

<ul>
  <li>utility depots</li>
  <li>outage events</li>
  <li>emergency response routes</li>
  <li>service coverage areas</li>
  <li>layer controls</li>
  <li>interactive popups</li>
</ul>

<p>
  <img src="outputs/screenshots/leaflet_webmap_full_interface" alt="Interactive Leaflet Web GIS" width="80%">
</p>

<hr>

<h2>Interactive Web Map</h2>

<p>
The interactive Leaflet application is available locally at:
</p>

<pre>
webmap/index.html
</pre>

<p>
Run locally using:
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

<p>
  <img src="outputs/screenshots/leaflet_webmap_full_interface.png" alt="Leaflet Web Map Full Interface" width="100%">
</p>

<hr>

<h2>QGIS Workflow</h2>

<p>
QGIS is used for:
</p>

<ul>
  <li>GeoPackage layer validation</li>
  <li>CRS verification</li>
  <li>cartographic styling</li>
  <li>route inspection</li>
  <li>service area visualization</li>
  <li>final map-layout preparation</li>
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
The workflow uses EPSG:26918 (NAD83 / UTM Zone 18N) for accurate distance-based GIS analysis in Washington, DC.
</p>

<p>
Layers are converted back to EPSG:4326 for GeoJSON export and Leaflet web mapping.
</p>

<h3>Routing Method</h3>

<p>
Emergency response routes are calculated using shortest-path transportation-network routing rather than straight-line distance analysis.
</p>

<h3>Spatial Storage Strategy</h3>

<p>
The project originally considered PostGIS integration. The workflow was redesigned to use GeoPackage and DuckDB Spatial to improve reproducibility and reduce infrastructure overhead.
</p>

<h3>Service Coverage Modeling</h3>

<p>
Service areas are modeled using simplified distance buffers around utility depots. These represent approximate operational coverage zones.
</p>

<hr>

<h2>Results and Operational Insights</h2>

<ul>
  <li>Network-based routing produces more realistic emergency response analysis than Euclidean distance.</li>
  <li>Service coverage zones reveal possible operational accessibility gaps.</li>
  <li>Infrastructure impact analysis identifies transportation segments near outage areas.</li>
  <li>DuckDB Spatial enables lightweight spatial SQL analytics without requiring a dedicated database server.</li>
  <li>The workflow demonstrates how open-source GIS tools can support operational emergency-response planning.</li>
</ul>

<hr>

<h2>Limitations</h2>

<ul>
  <li>Utility depots and outage locations are simulated.</li>
  <li>Traffic conditions are not modeled.</li>
  <li>Travel time analysis is not included.</li>
  <li>Road restrictions and vehicle constraints are simplified.</li>
  <li>Service coverage zones use Euclidean buffers rather than network service areas.</li>
</ul>

<hr>

<h2>Future Improvements</h2>

<ul>
  <li>Travel-time-based routing</li>
  <li>Network service area analysis</li>
  <li>Real-time traffic integration</li>
  <li>Road closure simulation</li>
  <li>Deployment through GitHub Pages</li>
  <li>Advanced QGIS cartographic layouts</li>
  <li>Reusable Python routing toolkit</li>
</ul>

<hr>

<h2>How to Run the Project</h2>

<h3>1. Clone Repository</h3>

<pre>
git clone git@github.com:namozhdehi/utility-emergency-response-routing-analysis.git
cd utility-emergency-response-routing-analysis
</pre>

<h3>2. Create Virtual Environment</h3>

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

<h3>5. Open Notebook</h3>

<pre>
notebooks/utility_emergency_routing_analysis.ipynb
</pre>

<h3>6. Launch Web Map</h3>

<pre>
cd webmap
python3 -m http.server 8000
</pre>

<hr>

<h2>Repository Notes</h2>

<p>
The repository excludes:
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
GIS and geospatial engineering portfolio project focused on transportation-network analysis, emergency routing workflows, spatial SQL, and interactive web GIS visualization.
</p>

# Stats NZ 'There and back again' Competition Entry

[Link](https://thangandrory.github.io/)
[Link to Source Code before Browserified]('https://github.com/thangpham7793/stat_nz_map_leaflet_js/tree/master/src')

Welcome to the tutorial document for my entry for the StatsNZ ‘There and back again’ data visualisation competition.

The app was built using a variety of Python and JavaScript libraries and plugins such as Leaflet, Pandas, Plotly (and more), with data from StatsNZ and OpenStreetMap. The statistical programming was done using Anaconda’s Jupyter notebooks Python environment with Pandas.

Much of the inspiration for this app was taken from the 2013 version of the StatsNZ commuter-view app. This app is focused on the same general principles, while adding in some newer technologies to make the app lighter, smoother, faster, more immersive and easier to use.

The app has a range of features to help users navigate the Stats NZ Work and Student commuter datasets:

### Manual Zoom In/out: 
This lets users manually zoom in and out of the map view. Zooming into a given region is automatic when a region label is clicked, but the manual zoom gives users more control. — The mouse wheel also controls manual zoom.

### Search by Area: 
This gives users the ability to search by their general area rather than having to locate it on the map or scale out from their address, saving them time and effort.

### Search by Address: 
Similar to ‘Search by area’, this allows users to search their address directly and start by zooming out from there as an alternative experience.

### Data set Selector: 
This allows users to toggle between the worker and student data set to get the same perspectives on different commuter types.

### Map type Selector: 
Similar to ‘Data set Selector’ this lets users toggle between the default ‘Street View’ map and the ‘2018 Area Boundaries map’ for extra boundary precision.

### Clear All Paths: 
This button removes all active ant-path animations on the map (ant-path function covered shortly).

### A Closer Look
There are many zoom levels avaialbe and there are variations of base zoom levels for addresses. This means that some address icon are not displayed (to avoid clutter) when others are.

To unfold further addresses, users can click the tabs containing the desired address location. This will zoom users into those address clusters at the appropriate level, display the address icons at their centroid, and notify the users that a click will activate the chart feature.

For fun and simplicity, the pointer itself contain sa custom icon based on the dominant form of transport for that address code (i.e if an address has drive_car_truck_or_van as the highest value column: icon = car icon, if its Walk_or_jog: icon = walking icon etc).

### Ant-Paths 
Ant-paths visualise commuter data for their associated address. They contain the direction, distance, location and volume of commutes. Outbound commutes are grey lines and flow outward, inbound commutes are red lines and flow inward. The Ant-paths have a hover to display values which can be made stable with a click to the line. All Ant-paths can be cleared by clicking the clear button at the bottom-left of the user menu.

### Charts 
To pull up the chart panel of an address, the user can click the addresses icon. This will render two pie charts on the right side of the window, one showing a breakdown of the mode of transport, and the other showing the commuting flows in and out of the address. Users can download the pie charts as high quality PNG image files.

### Prospective improvements
Have charts for landing view regions (on hover) giving aggregate stats for the region.

- Have a ‘Interesting Facts’ chart tab displaying a range of interesting statistics i.e ‘Fittest transport city’, ‘Greenest transport Region’ etc.

- Have tool-tip for searched residential addresses with statistics for area address on hover.

- Add chart type selection menu for users.

- Do more testing and fix bugs

### Sources
https://docs.google.com/document/d/1mP-KDqwYHfKRFx_A8bV0oPFUz_VB_IIeqKArRgyYjNQ/edit?usp=sharing

# CAISO Electricity LMP Mapper

This repository provides the source code for http://electricitymapper.appspot.com , a tool for visualizing the location marginal price (LMP) of electricity on the [CAISO] electricity grid.  The site is designed to take data from CAISO's [OASIS] API, allowing the users to upload a .csv of the data which they want to see visualized (following certain formatting requirements, based on the template csv provided).

The map is implemented using Leaflet.js, with the display/coloring/updating of nodes handled through D3.js. It was deployed using the Google App Engine

To Do's:
--------
  - Allow Json file upload
  - Allow toggling of satellite view (good for seeing power lines and generators)
  - Pull the transmission line layer from Open Streetmaps and overlay it
  - Allow upload/visualization of multiple price components in parallel, probably through multiple sub-maps. This would allow simultaneous visualization of the three components of LMP: Marginal Cost of Energy, Marginal Cost of Congestion, and Marginal Cost of Losses, providing a more transparent view of what's happening in the grid.
  - Allow users to define color scales, and provide handling for out-of-range colors (go to black and white colored nodes?). When a single hour provides an extreme price spike, it skews the scale so that normal diurnal fluctuations are hard to see.
  - Use CSS or something to make it look better.
  
Related:
  - [Cleanweb Berkeley CAISO Scraper:] Tools for scraping  for scraping the real-time and historical LMP data
  - Check out [my work] and [let me know] if you have suggested improvements!

License
----

MIT

[my work]:http://linkedin.com/in/emunsing
[CAISO]:http://www.caiso.com
[OASIS]:http://oasis.caiso.com
[Electricity Mapper]:http://electricitymapper.appspot.com
[ElectricityMapper github project]:https://github.com/emunsing/ElectricityMapper
[Cleanweb]:http://cleanweb.berkeley.edu
[Cleanweb Berkeley CAISO Scraper:]:https://github.com/cwBerkeley/code
[let me know]:http://www.twitter.com/EcoMunsing
[Pyiso:]:https://github.com/watttime/pyiso
[WattTime]:http://www.watttime.org/

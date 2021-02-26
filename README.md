# Measuring Global Multi-Scale Place Connectivity using Geotagged Social Media Data 

Shaped by human movement, place connectivity is quantified by the strength of spatial interactions among locations. For decades, spatial scientists have researched place connectivity, applications, and metrics. The growing popularity of social media provides a new data stream where spatial social interaction measures are largely devoid of privacy issues, easily assessable, and harmonized. In this study, we introduced a global multi-scale place connectivity index (PCI) based on spatial interactions among places revealed by geotagged tweets as a spatiotemporal-continuous and easy-to-implement measurement. The multi-scale PCI, demonstrated at the US county level, exhibits a strong positive association with SafeGraph population movement records (10% penetration in the US population) and Facebook’s social connectedness index (SCI), a popular connectivity index based on social networks. We found that PCI has a strong boundary effect and that it generally follows the distance decay, although this force is weaker in more urbanized counties with a denser population. Our investigation further suggests that PCI has great potential in addressing real-world problems that require place connectivity knowledge, exemplified with two applications: 1) modeling the spatial spread of COVID-19 during the early stage of the pandemic and 2) modeling hurricane evacuation destination choice. The methodological and contextual knowledge of PCI, together with the launched visualization platform and open-sourced PCI datasets at various geographic levels, are expected to support research fields requiring knowledge in human spatial interactions.

The following datasets are currenlty available for download in this Github repository (more PCI datasets will be added when avaiable): 

* World country level PCI for 2019
* Worldwide first-level subdivision PCI for 2019
* US metropolitan-level PCI for 2019
* US county-level PCI for 2018 and 2019
* New York City census tract level PCI for 2018 and 2019
* Los Angeles County census tract level PCI for 2018 and 2019
* Directional (or Asymmetrical) PCI, number of shared Twitter users between each place pair, and number of total observed Twitter users in each place are also included in each PCI dataset
* Aggregated US county level person-day movements derived from Twitter for 2019
* Aggregated US county level person-day movements derived from SafeGraph data for 2019

All PCI datasets are in CSV (Comma-Separated Values) format having the same columns: place_i , place_j, shared_users, place_i_users, place_j_users,pci, dir_pci

* place_i: id for place i (using FIPS for places for US county and tract, using ISO place code for other places).
* place_j: id for place j (using FIPS for places for US county and tract, using ISO place code for other places).
* shared_users: number of shared Twitter users between place i and place j.
* place_i_users: number of total observed users in place i during the specified time period.
* place_j_users: number of total observed users in place i during the specified time period.
* pci: place connective index compuated with Eq. 1 in the manuscript.
* dir_pci: place connective index compuated with Eq. A1 and Eq. A2 in the manuscript Appendix A. 

The interactive web portal for visualizing the PCI and relevant datasets can be accessed at http://gis.cas.sc.edu/GeoAnalytics/pci.html.

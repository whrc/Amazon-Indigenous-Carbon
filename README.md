[![DOI](https://zenodo.org/badge/199693162.svg)](https://zenodo.org/doi/10.5281/zenodo.10822438)

# Amazon-Indigenous-Carbon

This repository contains data central to the analysis reported by Walker et al. (2020) on the role of forest conversion, degradation, and disturbance in the carbon dynamics of Amazon indigenous territories and protected natural areas. These data include:

1. Two raster layers of aboveground live dry woody carbon spanning the biogeographic limit of the Amazon:
+ `Amazon_ACD_2003_500m_Mgha.tif` is a single-band GeoTIFF in which grid cells reflect aboveground carbon density for baseline year 2003.
+ `Amazon_ACD_Change_2003_2016_500m_Mgha.tif` is a 13-band GeoTIFF in which grid cells reflect annual aboveground carbon density change for the 2003-2016 time period (i.e., band 1 = 2003-2004; band 13 = 2015-2016). Only pixels exhibiting statistical significance at the 95% level are reported.

The spatial resolution is ca. 500 meters and the coordinate reference system is the MODIS sinusoidal projection ([SR-ORG:6842](https://spatialreference.org/ref/sr-org/modis-sinusoidal/)). Grid cell values are stored as 16-bit signed integers with units of megagrams of aboveground carbon per hectare (Mg/ha). Areas outside the biogeographical limit of the Amazon are assigned to NoData (-32768).

2. One vector layer containing the spatial distribution (ca. 2016) of Indigenous Territories (ITs), Protected Natural Areas (PNAs), IT/PNA Overlap, and Other Land categories within the biogeographic limit of the Amazon:
+ `msk_paises.gdb.tar.gz` is a compressed ESRI geodatabase containing a polygon feature class in which the "TIPO_UND" field indicates the land category (i.e., 1 = IT; 2 = PNA; 3 = IT/PNA Overlap; 4 = Other Land) and the "Pais" field indicates the three-letter ISO country code (e.g., "BOL" = Bolivia) of each polygon.

This work is licensed under a  [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](http://creativecommons.org/licenses/by-nc-nd/4.0/). You may not use these data for commercial purposes; if you transform or build upon these data, you may not distribute the modified data. You must cite this paper (i.e., Walker et al. 2020) when using any of these datasets for any purpose.

## Data Source

Walker, W.S., S.R. Gorelik, A. Baccini, J.L. Aragon-Osejo, C. Josse, C. Meyer, M.N. Macedo, C. Augusto, S. Rios, T. Katan, A.A. de Souza, S. Cuellar, A. Llanos, I. Zager, G.D. Mirabal, K.K. Solvik, M.K. Farina, P. Moutinho, and S. Schwartzman. 2020. **The role of forest conversion, degradation, and disturbance in the carbon dynamics of Amazon indigenous territories and protected areas.** _Proceedings of the National Academy of Sciences_, [doi:10.1073/pnas.1913321117](https://doi.org/10.1073/pnas.1913321117).

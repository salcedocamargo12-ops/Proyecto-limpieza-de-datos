# Annual CO₂ emissions - Data package

This data package contains the data that powers the chart ["Annual CO₂ emissions"](https://ourworldindata.org/grapher/annual-co2-emissions-per-country?v=1&csvType=full&useColumnShortNames=false) on the Our World in Data website. It was downloaded on November 19, 2026.

### Active Filters

A filtered subset of the full data was downloaded. The following filters were applied:

## CSV structure

Each row is an observation for an entity (usually a country or region) at a timepoint.

- "Entity" — the name of the entity, e.g. "United States".
- "Code" — our internal entity code. For most countries this is the [ISO alpha-3](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3) code, e.g. "USA"; historical and other non-standard entities get a custom code.
- "Year" or "Day" — the timepoint. Annual data has a "Year" column holding an integer year; otherwise a "Day" column holds a date string in the form "YYYY-MM-DD".
- The final column is the data column — the time series that powers the chart. Downloaded with the "full data" option it corresponds to the time series below; with "only selected data visible in the chart" it is transformed depending on the chart type, so the correspondence may be less direct.


## Metadata.json structure

The .metadata.json file contains metadata about the data package. The "charts" key contains information to recreate the chart, like the title, subtitle etc. The "columns" key contains information about each of the columns in the csv, like the unit, timespan covered, citation for the data etc.

## How we process data at Our World in Data

Our World in Data is almost never the original producer of the data - almost all of the data we use has been compiled by others. If you want to re-use data, it is your responsibility to ensure that you adhere to the sources' license and to credit them correctly. Please note that a single time series may have more than one source - e.g. when we stitch together data from different time periods by different producers or when we calculate per capita metrics using population data from a second source.

Preparing this data involves several processing steps. Depending on the data, this can include standardizing country names and world region definitions, converting units, calculating derived indicators such as per capita measures, as well as adding or adapting metadata such as the name or the description given to an indicator.
[Read about our data pipeline](https://docs.owid.io/projects/etl/).

## Detailed information about the data


### Annual CO₂ emissions
Annual total emissions of carbon dioxide (CO₂), excluding land-use change, measured in tonnes.
Last updated: November 10, 2026  
Next expected update: November 2027  
Date range: 1750–2025  
Unit: tonnes  
Source: Global Carbon Budget (2026) – with major processing by Our World in Data  

#### How to cite this data

Global Carbon Budget (2026) – with major processing by Our World in Data

#### What you should know about this data
- This data is based on territorial emissions, meaning the emissions produced within a country's borders, but not those from imported goods. For example, emissions from imported steel are counted in the country where the steel is produced. To learn more and look at emissions adjusted for trade, read our article: [How do CO₂ emissions compare when we adjust for trade?](https://ourworldindata.org/consumption-based-co2)
- Emissions from international aviation and shipping are not included in the data for any individual country or region. They are only counted in the global total.

#### Notes on our processing step for this indicator
- Global emissions are converted from tonnes of carbon to tonnes of carbon dioxide (CO₂) using a factor of 3.664. This is the conversion factor [recommended by the Global Carbon Project](https://globalcarbonbudget.org/download/2454/). It reflects that one tonne of carbon, when fully oxidized, forms 3.664 tonnes of CO₂, based on the relative molecular weights of carbon and oxygen in CO₂.
- Emissions from the 1991 Kuwaiti oil fires are included in Kuwait's emissions for that year.


## Sources

These are the sources behind the data in this package. Each time series above names the ones it draws on in its citation.

### Global Carbon Project – Global Carbon Budget

The Global Carbon Budget was established by the Global Carbon Project (GCP) to track global carbon emissions and sinks.

This dataset makes it possible to assess whether countries are making progress toward the goals of the Paris Agreement and is widely recognized as the most comprehensive report of its kind.

Since 2001, the GCP has published estimates of global and national fossil CO₂ emissions. Initially, these were simple republished data from other sources, but over time, refinements were made based on feedback and correction of inaccuracies.

Producer: Global Carbon Project  
Published: 2026-11-10  
Retrieved on: 2026-11-05  
Retrieved from: https://globalcarbonbudget.org/  
Direct download: https://zenodo.org/records/23667912/files/GCB2026v11_MtCO2_flat.csv?download=1  
License: CC BY 4.0 (https://doi.org/10.5281/zenodo.5569234)  

Citation: Andrew, R. M., & Peters, G. P. (2026). The Global Carbon Project's fossil CO2 emissions dataset (2026v11) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.23667912

The data files of the Global Carbon Budget can be found at: https://globalcarbonbudget.org/carbonbudget/

For more details, see the original paper:
Friedlingstein, P., O'Sullivan, M., Jones, M. W., Andrew, R. M., Bakker, D. C. E., Hauck, J., Landschützer, P., Le Quéré, C., Li, H., Luijkx, I. T., Peters, G. P., Peters, W., Pongratz, J., Schwingshackl, C., Sitch, S., Canadell, J. G., Ciais, P., Aas, K., Alin, S. R., Anthoni, P., Barbero, L., Bates, N. R., Bellouin, N., Benoit-Cattin, A., Berghoff, C. F., Bernardello, R., Bopp, L., Brasika, I. B. M., Chamberlain, M. A., Chandra, N., Chevallier, F., Chini, L. P., Collier, N. O., Colligan, T. H., Cronin, M., Djeutchouang, L. M., Dou, X., Enright, M. P., Enyo, K., Erb, M., Evans, W., Feely, R. A., Feng, L., Ford, D. J., Foster, A., Fransner, F., Gasser, T., Gehlen, M., Gkritzalis, T., Goncalves De Souza, J., Grassi, G., Gregor, L., Gruber, N., Guenet, B., Gürses, Ö., Harrington, K., Harris, I., Heinke, J., Hurtt, G. C., Iida, Y., Ilyina, T., Ito, A., Jacobson, A. R., Jain, A. K., Jarníková, T., Jersild, A., Jiang, F., Jones, S. D., Kato, E., Keeling, R. F., Klein Goldewijk, K., Knauer, J., Kong, Y., Korsbakken, J. I., Koven, C., Kunimitsu, T., Lan, X., Liu, J., Liu, Z., Liu, Z., Lo Monaco, C., Ma, L., Marland, G., McGuire, P. C., McKinley, G. A., Melton, J. R., Monacci, N., Monier, E., Morgan, E. J., Munro, D. R., Müller, J. D., Nakaoka, S.-I., Nayagam, L. R., Niwa, Y., Nutzel, T., Olsen, A., Omar, A. M., Pan, N., Pandey, S., Pierrot, D., Qin, Z., Regnier, P., Rehder, G., Resplandy, L., Roobaert, A., Rosan, T. M., Rödenbeck, C., Schwinger, J., Skjelvan, I., Smallman, T. L., Spada, V., Sreeush, M. G., Sun, Q., Sutton, A. J., Sweeney, C., Swingedouw, D., Séférian, R., Takao, S., Tatebe, H., Tian, H., Tian, X., Tilbrook, B., Tsujino, H., Tubiello, F., van Ooijen, E., van der Werf, G. R., van de Velde, S. J., Walker, A. P., Wanninkhof, R., Yang, X., Yuan, W., Yue, X., and Zeng, J.: Global Carbon Budget 2025, Earth Syst. Sci. Data, 18, 3211-3288, https://doi.org/10.5194/essd-18-3211-2026, 2026.

    
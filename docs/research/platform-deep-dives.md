# Existing Platform Deep-Dive

## Project
Africa Climate Intelligence

## Research Stage
Week 2 — Competitor and ecosystem research

## Day
Day 10 — Deep-dive existing platforms

---

# 1. Purpose

This document examines existing climate, weather, geospatial and
humanitarian-information platforms relevant to Kenya and East Africa.

The objective is to understand:

- who the platforms serve;
- what information they provide;
- how users access the information;
- technical requirements;
- data formats and interoperability;
- visualization and analysis capabilities;
- pricing/access models;
- operational models;
- strengths;
- limitations or workflow friction;
- potential overlap with Africa Climate Intelligence.

A limitation or gap identified here is treated as a research hypothesis
until validated with actual users.

---

# 2. Platform Classification

The platforms examined are not all direct competitors.

They fall into several categories:

1. National climate-information provider
2. Regional climate-information provider
3. Global climate-information platform
4. Technical climate-data infrastructure
5. Humanitarian/development data platform

This distinction is important because Africa Climate Intelligence may
eventually complement existing data providers rather than replace them.

---

# 3. Platform 1 — Kenya Meteorological Department (KMD)

## Type

National meteorological and climate-information provider.

## Primary role

KMD manages meteorological and climate information for Kenya and
provides climate information services to users.

## Target users

Potential and documented users include:

- government;
- decision-makers;
- researchers;
- development organizations;
- climate-sensitive sectors;
- humanitarian/early-warning actors;
- other users requiring Kenyan weather and climate information.

## Main services

KMD provides:

- meteorological observations;
- climate data;
- climate information;
- forecasts;
- climate monitoring;
- climate-information services;
- Maprooms.

KMD's Climate Data Management Services manages climate data from
meteorological observation systems operated by KMD and partner systems.

## Data sources

KMD receives data from:

- meteorological observation systems;
- automatic weather stations;
- partner observation systems;
- other reporting mechanisms.

The data goes through initial and further quality-control processes
before being archived.

## Maprooms

KMD operates Climate Information Service Maprooms.

The Maprooms combine station information with satellite estimates
for rainfall and station/reanalysis information for other weather
parameters.

Users can explore information at:

- national level;
- regional level;
- county;
- sub-county;
- ward;
- grid-point levels.

## Access

KMD has multiple access mechanisms.

The KMD Climate Information Service Maprooms are available through
a web portal.

KMD also states that climate-data requests can be submitted through
the Kenyan e-Citizen system.

## Visualization

Strong visualization component through Maprooms.

Users can explore climate information spatially and temporally.

## GIS relevance

High.

The Maprooms allow spatial exploration and analysis at different
administrative levels and grid points.

## API

An API should be investigated separately during technical research.
The current research does not assume that all KMD information is
available through an open API.

## Pricing/access

Access is not treated as universally "free".

KMD's current data-access process includes formal data requests through
e-Citizen.

Specific datasets, services and licensing/payment conditions need to be
verified before commercial use.

## Operational model

Government-operated national meteorological service.

## Strengths

- authoritative national source;
- Kenya-specific observations;
- national geographic coverage;
- quality-control processes;
- climate-information services;
- Maproom visualization;
- information at useful administrative levels;
- strong relevance for decision-making.

## Potential workflow friction to investigate

- Difference between browsing information and obtaining underlying data;
- formal data-request process;
- availability of machine-readable/API access;
- ability to combine KMD information with external datasets;
- ability to perform customized analysis;
- interoperability with GIS and organizational datasets.

These are hypotheses requiring user validation.

## Potential overlap with Africa Climate Intelligence

Africa Climate Intelligence should not assume it should reproduce
KMD's observation or forecasting role.

Potential overlap would be strongest if the proposed platform attempted
to become another general Kenyan weather-information portal.

## Potential complementarity

Potentially:

KMD data/services
+
other climate datasets
+
GIS/contextual datasets
+
workflow tools
=
decision-oriented information.

This requires validation and licensing review.

## Evidence

KMD Climate Data Management documentation and State of the Climate
report.

---

# 4. Platform 2 — ICPAC

## Type

Regional climate-information and climate-services institution.

## Geographic focus

Greater Horn of Africa / Eastern Africa.

## Primary role

ICPAC provides regional climate monitoring, forecasting, data services,
early-warning information and climate applications.

## Target users

Potential users include:

- national meteorological services;
- governments;
- researchers;
- development organizations;
- humanitarian organizations;
- disaster-risk practitioners;
- agriculture and food-security organizations;
- environmental organizations;
- other climate-sensitive sectors.

## Data services

ICPAC provides regional climate datasets including:

- precipitation;
- mean temperature;
- maximum temperature;
- minimum temperature.

Datasets can be available at:

- daily;
- 10-day;
- monthly;
- seasonal;
- annual

temporal scales.

## Data Center

The ICPAC Data Center includes applications such as:

- Climate Data;
- Geoportal;
- Environmental Data;
- Agriculture Watch;
- Hazards Watch;
- WMO RCC;
- MESA Geoportal.

## Dataset categories

The Data Center includes:

### Climate

- precipitation;
- temperature.

### Environmental monitoring

- vegetation;
- fires.

### Agriculture and food security

- soil.

### Other products

- land-surface temperature;
- evapotranspiration;
- soil moisture;
- vegetation indicators.

## Spatial and temporal filtering

The Data Center supports filtering by:

- geographic extent;
- temporal resolution;
- spatial resolution;
- data format.

Examples of available spatial resolutions include approximately:

- 300 m;
- 1 km;
- 3 km;
- 4 km;
- 8 km;
- 10 km;
- 11 km;
- 25 km.

Some datasets are available as GeoTIFF.

## Example — CHIRPS

ICPAC provides access to CHIRPS precipitation products.

CHIRPS is a long-term rainfall dataset incorporating satellite imagery
and station data.

ICPAC provides derived products including:

- rainfall totals;
- averages;
- minimum/maximum statistics;
- anomalies;
- normalized precipitation;
- monthly products.

## Access

ICPAC provides a Data Center and data-service mechanisms.

Some data can be downloaded through the platform, while other data
services involve formal data requests.

## Visualization

Strong.

ICPAC provides:

- climate monitoring products;
- maps;
- climate applications;
- geoportal functionality;
- monitoring dashboards/products.

## API

Technical/API access varies by service and dataset.

This needs dataset-level investigation rather than assuming a single
ICPAC API covers everything.

## Pricing/access

Mixed depending on dataset/service.

Access conditions and licensing should be checked individually.

## Operational model

Regional intergovernmental climate centre under IGAD.

ICPAC is also designated as a WMO Regional Climate Centre.

## Strengths

- regional geographic coverage;
- strong East Africa relevance;
- multiple climate datasets;
- environmental monitoring;
- agriculture/food-security applications;
- climate monitoring;
- early-warning relevance;
- GIS-compatible datasets;
- multiple temporal/spatial resolutions.

## Potential workflow friction to investigate

- Multiple datasets with different characteristics;
- different data formats;
- dataset discovery;
- combining datasets;
- processing GeoTIFF/raster data;
- moving from monitoring products to organization-specific analysis;
- integration with programme/project data;
- technical skill requirements.

These are hypotheses, not confirmed user problems.

## Potential overlap

A platform attempting to become another regional climate-data
repository could substantially overlap with ICPAC.

## Potential complementarity

Potential areas to investigate:

- easier cross-source discovery;
- integration of multiple datasets;
- contextualization for specific users;
- workflow support;
- linking climate information to programme/project data;
- decision-ready outputs.

Any use of ICPAC data would require checking access and licensing.

## Evidence

ICPAC Data Center and Data Services documentation.

---

# 5. Platform 3 — World Bank Climate Change Knowledge Portal (CCKP)

## Type

Global climate-information platform focused strongly on development
and climate-risk analysis.

## Primary users

The platform is particularly relevant to:

- development practitioners;
- policymakers;
- researchers;
- climate-risk analysts.

## Main purpose

Provides historical climate information, climate projections and
related climate-risk information.

## Historical data

CCKP provides historical climate information based on sources such as:

- CRU;
- ERA5.

The portal allows users to examine:

- spatial variation;
- seasonal cycles;
- time series;
- climate trends;
- variability.

## Future climate information

CCKP provides CMIP6-based climate projections.

Users can explore different scenarios and projection periods.

## Geographic coverage

The platform supports:

- countries;
- subnational administrative areas;
- watersheds;
- other geographic units depending on the product.

## Data access

CCKP provides:

- interactive visualization;
- spatially aggregated downloads;
- gridded NetCDF files;
- API access.

## API

CCKP provides an API structure for querying climate data by:

- dataset;
- variable;
- product;
- aggregation;
- period;
- scenario;
- model;
- geographic unit.

This is technically important because it makes CCKP more than a
visualization-only platform.

## Data formats

Examples include:

- NetCDF;
- JSON/API;
- Excel outputs.

## Visualization

Strong.

Users can examine:

- maps;
- time series;
- seasonal cycles;
- climate trends;
- variability;
- projections.

## Pricing/access

The portal provides broad access to its climate information and
downloads.

Individual underlying datasets have their own provenance and
conditions.

## Operational model

International development institution/platform.

## Strengths

- development-oriented framing;
- country and subnational analysis;
- historical and future climate;
- strong visualization;
- downloadable data;
- API access;
- multiple climate datasets;
- climate-risk context.

## Potential workflow friction to investigate

- Users may still need to combine CCKP information with local
  programme/project datasets.
- API and gridded data may require technical knowledge.
- Different products may require understanding of climate-data
  terminology.
- Users working specifically in Kenya may need additional local
  datasets.

These are hypotheses.

## Potential overlap

A general climate-data visualization and download platform would overlap
with CCKP.

## Potential complementarity

A Kenya-focused workflow that integrates climate information with
specific organizational/project contexts could potentially complement
rather than replace CCKP.

## Evidence

World Bank Climate Change Knowledge Portal documentation and data
download/API documentation.

---

# 6. Platform 4 — Copernicus Climate Data Store (CDS)

## Type

Large-scale technical climate-data infrastructure.

## Primary users

Particularly relevant to:

- researchers;
- data scientists;
- developers;
- climate analysts;
- technical organizations.

## Main purpose

Provides access to large collections of climate datasets and tools.

## Data

The CDS provides access to datasets across climate monitoring,
reanalysis and climate-change applications.

A major example is ERA5 reanalysis.

## Access

Users can obtain data:

1. interactively through the web interface;
2. programmatically through APIs.

## API

The CDS provides programmatic access through its API.

Users need:

- an account;
- personal access credentials/token;
- API client setup;
- knowledge of the dataset and request parameters.

Python is supported through the `cdsapi` client.

## Technical requirements

Programmatic access requires understanding of:

- Python;
- API requests;
- dataset identifiers;
- request parameters;
- data formats;
- authentication;
- terms of use.

## Visualization

The platform provides interactive data access and applications, while
technical users can also process the datasets using external tools.

The wider Copernicus ecosystem includes tools such as earthkit and
JupyterHub for processing and analysis.

## Data processing

Users may need to:

- select datasets;
- construct requests;
- download files;
- process them;
- analyse them;
- visualize them externally.

## Pricing/access

The CDS provides broad access to datasets, but individual datasets
have terms of use that must be accepted before downloading.

## Operational model

Large international scientific/technical infrastructure operated within
the Copernicus Climate Change Service ecosystem.

## Strengths

- extensive datasets;
- strong scientific infrastructure;
- programmatic access;
- documentation;
- Python tooling;
- large technical ecosystem;
- powerful data-selection capabilities.

## Potential workflow friction to investigate

- technical complexity;
- dataset discovery;
- authentication;
- request construction;
- data processing;
- large files;
- need for external analysis tools;
- expertise required to interpret datasets.

These are not necessarily weaknesses for the intended technical user;
they may simply reflect the platform's design for advanced users.

## Potential overlap

Africa Climate Intelligence should not attempt to reproduce the
underlying global climate-data infrastructure.

## Potential complementarity

Potentially:

CDS
+
other climate sources
+
Kenya-specific contextual datasets
+
simplified workflows
+
decision-oriented outputs.

This is a hypothesis requiring validation.

## Evidence

Copernicus Climate Data Store user guide and API documentation.

---

# 7. Platform 5 — Humanitarian Data Exchange (HDX)

## Type

Humanitarian/development data discovery and sharing platform.

## Why it is included

HDX is not primarily a climate-data platform.

It is included because our provisional target users include
humanitarian and development organizations.

It provides a useful model for studying how multiple organizations
can discover and work with data.

## Target users

- humanitarian organizations;
- UN agencies;
- NGOs;
- governments;
- researchers;
- analysts;
- developers;
- data practitioners.

## Main purpose

HDX aims to make humanitarian data easier to find and use.

## Data

HDX brings together datasets from many organizations covering:

- humanitarian operations;
- population;
- administrative boundaries;
- affected populations;
- food security;
- health;
- climate/hazards;
- operational presence;
- other humanitarian information.

## Discovery

Users can search by:

- country;
- crisis;
- organization;
- dataset;
- topic.

## API

HDX has:

- CKAN API;
- HDX HAPI;
- programmatic access mechanisms.

## HAPI

The HDX Humanitarian API standardizes indicators from multiple sources
to support automated workflows and visualizations.

The API supports filtering by:

- country;
- administrative area;
- sector;
- organization;
- other parameters depending on the endpoint.

## Data processing

HDX HAPI pipelines process incoming data and standardize elements
such as geographic codes and organizational/sector terminology.

## Formats

Depending on the dataset/API:

- CSV;
- JSON;
- XLSX;
- other source formats.

## Visualization

HDX supports data discovery and has associated visualization/API
products.

However, users can still need external tools for analysis and
custom visualization.

## Pricing/access

HDX is fundamentally an open humanitarian-data sharing platform.

Specific datasets can have their own conditions.

## Operational model

Managed by OCHA's Centre for Humanitarian Data.

Data is supplied by participating organizations and pipelines.

## Strengths

- large multi-organization ecosystem;
- strong discovery;
- standardized metadata;
- APIs;
- humanitarian focus;
- geographic filtering;
- organization-level data;
- interoperability efforts;
- automated data pipelines.

## Potential workflow friction to investigate

- climate data may exist in separate specialized platforms;
- users may still need to combine humanitarian datasets with climate
  datasets;
- data quality and update frequency can vary by source;
- external analysis may still be required;
- different platforms can use different schemas and standards.

## Potential overlap

A generic humanitarian data repository would overlap with HDX.

## Potential complementarity

A climate-focused system designed specifically to connect climate
information with humanitarian/development workflows could potentially
sit alongside HDX.

For example:

HDX humanitarian data
+
KMD/ICPAC climate information
+
geospatial/contextual data
=
climate-risk analysis workflow.

Whether users actually need this should be tested.

## Evidence

HDX platform documentation, HAPI documentation and HDX technical
documentation.

---

# 8. Cross-Platform Comparison

| Platform | Primary role | Main users | Data | Access | API | Visualization | Technical level | Cost/access | Operational model |
|---|---|---|---|---|---|---|---|---|---|
| KMD | National climate/weather services | Government, researchers, sectors, decision-makers | Kenya weather/climate | Web + formal data requests | Needs dataset-level verification | Strong | Low–medium depending on task | Mixed; verify by service | Government |
| ICPAC | Regional climate services | Governments, humanitarian/development, researchers | Climate, environmental, agriculture, hazards | Web/data services | Varies by service | Strong | Medium–high | Mixed; verify by dataset | Regional intergovernmental |
| CCKP | Climate/development information | Development, policy, research | Historical + projections | Web + downloads + API | Yes | Strong | Medium | Broad access; verify underlying data terms | International development institution |
| Copernicus CDS | Climate-data infrastructure | Researchers, developers, analysts | Large climate/reanalysis collections | Web + API | Yes | Moderate/strong ecosystem | High | Broad access; dataset terms apply | International scientific infrastructure |
| HDX | Humanitarian data discovery | Humanitarian/development/data users | Multi-sector humanitarian data | Web + API | Yes | Moderate | Low–high depending on task | Open platform; dataset conditions vary | OCHA-managed |

---

# 9. Platform Categories

## Direct competitors

Not yet established.

A platform should only be classified as a direct competitor after
user research confirms that users consider it an alternative solution
to the problem we are trying to solve.

## Indirect competitors

Potential examples:

- KMD;
- ICPAC;
- CCKP;
- HDX;
- specialized climate-data platforms.

They may solve portions of the problem.

## Substitutes

Users may currently substitute:

- Google searches;
- Excel;
- QGIS;
- ArcGIS;
- Python;
- institutional databases;
- internal dashboards;
- manually maintained spreadsheets;
- reports and PDFs.

These are particularly important because the real competition may not
be another website.

## Infrastructure/data providers

Potential examples:

- KMD;
- ICPAC;
- Copernicus;
- CHIRPS;
- NASA;
- NOAA;
- other Earth-observation and climate-data providers.

---

# 10. What Existing Platforms Already Do Well

The research shows that the ecosystem already has significant
capabilities.

Existing platforms can provide:

- authoritative observations;
- regional climate datasets;
- historical climate information;
- climate projections;
- climate monitoring;
- environmental monitoring;
- geospatial data;
- APIs;
- data downloads;
- maps;
- dashboards;
- humanitarian datasets;
- standardized geographic information;
- programmatic access.

Therefore, the project's problem cannot simply be:

> "Climate data is unavailable."

A stronger hypothesis is:

> "Climate information exists across multiple systems, but users may
> still experience difficulty discovering, combining, processing and
> applying the information to specific research, humanitarian,
> development or operational decisions."

This hypothesis requires primary-user validation.

---

# 11. Potential Workflow Friction

The following should currently be treated as hypotheses:

### A. Fragmentation

Users may need to visit multiple platforms to answer one question.

### B. Dataset discovery

Finding the correct dataset may require technical or domain knowledge.

### C. Interoperability

Datasets may differ in:

- format;
- resolution;
- temporal scale;
- geographic structure;
- naming conventions;
- metadata.

### D. Processing

Users may need to perform:

- downloads;
- extraction;
- clipping;
- conversion;
- reprojection;
- aggregation;
- cleaning;
- joins.

### E. Contextualization

Climate data may need to be combined with:

- population;
- infrastructure;
- programme locations;
- administrative boundaries;
- vulnerability;
- environmental information.

### F. Technical barriers

Some powerful platforms are designed for technically capable users.

### G. From data to decision

A platform may successfully provide data without providing the
workflow needed to turn that data into a decision-ready product.

---

# 12. Emerging Product Hypotheses

These are NOT product decisions.

They are hypotheses to test through interviews.

## Hypothesis 1 — Discovery layer

Users may benefit from one place to discover relevant climate datasets
across multiple providers.

## Hypothesis 2 — Integration layer

Users may benefit from combining climate data with contextual
geospatial and programme data.

## Hypothesis 3 — Workflow layer

Users may benefit from tools that reduce repetitive data preparation
and GIS processing.

## Hypothesis 4 — Decision layer

Users may value information presented around a specific decision or
use case rather than raw datasets.

## Hypothesis 5 — Kenya-first approach

A Kenya-focused initial product may be more useful than immediately
attempting to cover the entire African continent.

This remains consistent with our current project strategy.

---

# 13. Important Strategic Observation

Existing platforms are not necessarily evidence that the project should
not exist.

They demonstrate that:

- climate data infrastructure already exists;
- significant investment has already been made;
- users already have multiple tools;
- the project should avoid unnecessary duplication.

The potential opportunity, if validated, may therefore be in the
**workflow between existing information providers and users**.

Potential architecture:

DATA PROVIDERS
    ↓
KMD / ICPAC / CCKP / Copernicus / EO / humanitarian datasets
    ↓
AFRICA CLIMATE INTELLIGENCE
    ↓
Discovery
Integration
Processing
Analysis
Visualization
Decision support
    ↓
Researchers / NGOs / humanitarian / development users

This is only a working hypothesis.

---

# 14. Questions to Validate with Users

## Researchers

1. How do you find climate data?
2. Which platforms do you use most?
3. How many sources do you normally combine?
4. What happens after you download the data?
5. What processing is required?
6. Which step takes the most time?
7. What makes you trust one dataset over another?

## NGOs / humanitarian / development organizations

1. What climate information do you actually use?
2. Where do you obtain it?
3. What decisions does it support?
4. How do you combine it with programme data?
5. Who performs the analysis?
6. How long does the process normally take?
7. What information is difficult to obtain?
8. What information arrives too late to be useful?
9. What do you currently do manually?
10. What would make the workflow easier?

## Developers

1. Which climate/weather APIs do you use?
2. What makes climate-data integration difficult?
3. How good is the documentation?
4. How easy is historical data access?
5. What formats cause problems?
6. How important are licensing terms?
7. What prevents reliable production use?
8. What would make an African climate-data API more useful?

---

# 15. Day 10 Conclusion

The competitive/ecosystem research does NOT currently demonstrate
that there is an obvious empty market.

Instead, it shows a relatively mature but fragmented ecosystem with
different platforms serving different layers.

The key research question therefore becomes:

> Can Africa Climate Intelligence provide enough additional value by
> making existing climate information easier to discover, combine,
> analyse and apply to Kenya-specific research, humanitarian,
> development and operational decisions?

This must be tested with users before committing to a product direction.

---

# 16. Sources

## Kenya Meteorological Department

- Climate Data Management Services
- State of the Climate in Kenya 2025
- KMD Climate Information Service / Maprooms

## ICPAC

- ICPAC Data Center
- ICPAC Data Services
- ICPAC Climate Monitoring
- ICPAC dataset documentation

## World Bank

- Climate Change Knowledge Portal
- CCKP historical climate information
- CCKP data download/API documentation

## Copernicus

- Climate Data Store
- CDS User Guide
- CDS API documentation

## HDX

- Humanitarian Data Exchange
- HDX HAPI documentation
- HDX CKAN API documentation
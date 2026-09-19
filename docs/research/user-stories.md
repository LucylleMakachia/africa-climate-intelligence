# Day 6 — Three User Stories

## Purpose

These user stories represent three potential user groups for the Africa Climate Intelligence platform. They are hypotheses to be validated through user research and are not yet confirmed product requirements.

---

## 1. Researcher

### User Story

**As a** climate, environmental, GIS, or development researcher,

**I want to** discover, access, understand and analyze weather and climate datasets for Kenya,

**so that** I can conduct research without spending excessive time locating, cleaning, understanding and combining data from different sources.

### Potential Needs

* Dataset discovery
* Historical climate data
* Metadata
* Spatial data
* Time-series data
* Download/API access
* Data provenance
* Documentation
* GIS-compatible formats
* Dataset comparison

### Problem Hypothesis

Researchers may spend considerable time navigating multiple data providers and understanding differences in datasets, formats, spatial resolution and metadata.

### Validation Questions

* Which sources do researchers currently use?
* What takes the most time?
* Which datasets are difficult to find?
* What metadata do they need?
* Do they need analysis tools or primarily data access?
* Would they use an aggregation platform?

---

## 2. NGO / Consultant

### User Story

**As an** NGO programme, M&E, GIS, climate-resilience, humanitarian, or environmental consultant working in Kenya,

**I want to** quickly obtain and use weather, climate, hazard and geographic information for the areas where I work,

**so that** I can support project planning, monitoring, risk assessment, mapping, reporting and decision-making.

### Potential Needs

* Location-specific information
* Weather and climate indicators
* Hazard information
* Maps
* Historical trends
* Forecasts
* Project-location analysis
* Downloadable data
* Automated reports
* GIS integration
* Multiple data sources

### Problem Hypothesis

Organizations may need to combine information from several specialized systems when preparing project analysis, maps, reports or risk assessments.

### Validation Questions

* What information do organizations use?
* Which platforms do they currently use?
* How many sources are involved?
* What manual processing is required?
* How frequently is the workflow repeated?
* What outputs do they produce?
* Would they pay for time savings or specialized analysis?

---

## 3. Developer

### User Story

**As a** developer building a climate, environmental, humanitarian, agricultural or GIS application,

**I want to** access reliable, well-documented and programmatically accessible weather and climate data,

**so that** I can integrate climate information into applications without manually downloading and processing datasets.

### Potential Needs

* APIs
* Documentation
* Authentication
* Stable endpoints
* JSON/CSV/GeoJSON
* Raster access
* Geospatial services
* Metadata
* Data dictionaries
* Rate limits
* Versioning
* Licensing information
* Example code

### Problem Hypothesis

Climate information can be distributed across different systems with different APIs, formats, access requirements and licensing conditions.

### Validation Questions

* Which APIs do developers currently use?
* What makes a climate API difficult to work with?
* Which formats are preferred?
* What reliability requirements exist?
* What documentation is missing?
* Which datasets would developers actually integrate?
* Would developers pay for simplified APIs or processed datasets?

---

# Cross-User Comparison

| User             | Primary Job                      | Potential Pain Point               | Potential Value               |
| ---------------- | -------------------------------- | ---------------------------------- | ----------------------------- |
| Researcher       | Find and analyze data            | Discovery, metadata and processing | Faster research               |
| NGO / Consultant | Apply information to projects    | Fragmented sources and workflows   | Faster analysis and reporting |
| Developer        | Integrate data into applications | APIs, formats and documentation    | Easier integration            |

## Current Hypothesis

The three groups represent different potential forms of value:

**Researcher:** Find → Understand → Analyze

**NGO / Consultant:** Find → Combine → Apply → Report

**Developer:** Discover → Access → Integrate → Build

These user stories should be treated as hypotheses until validated through interviews, workflow observation and prototype testing.

## Relationship to the Day 5 Primary Segment

The Day 5 project decision identified **humanitarian and development organizations working in Kenya** as the provisional primary organizational/customer segment.

The Day 6 user stories deliberately examine three different potential user types — **researchers, NGO/consultants, and developers** — to avoid prematurely assuming that every potential user has the same needs.

The NGO/consultant user story is the closest match to the current primary segment. Researchers and developers are being examined as adjacent potential users who may interact with the platform independently or support humanitarian/development organizations.

Further user research will determine:

1. Which user group experiences the strongest recurring problem.
2. Whether the primary customer should remain humanitarian/development organizations.
3. Whether researchers or developers represent secondary customer segments.
4. Whether different users require different products, features, or pricing models.

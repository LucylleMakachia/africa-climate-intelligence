# User Workflows

## Africa Climate Intelligence

**Research stage:** Week 2 — Competitor and ecosystem research
**Day:** Day 11 — Current user workflows
**Status:** Working analysis — requires primary-user validation

---

## 1. Purpose

This document maps how potential users may currently move from a climate/weather information need to a useful output.

The purpose is to understand:

* where users obtain information;
* which platforms they use;
* what tools they use;
* how datasets move between systems;
* where manual work occurs;
* where users depend on technical specialists;
* where information may be difficult to interpret or apply;
* which potential friction points should be tested through interviews.

The workflows in this document are **working hypotheses** based on ecosystem and platform research. They should not be treated as confirmed descriptions of every user's workflow.

---

# 2. Target User Groups

The current research focuses on three user groups:

1. **Researcher**
2. **NGO / humanitarian / development professional**
3. **Developer / data professional**

The NGO/humanitarian/development group remains the project's **provisional primary user segment**.

This classification will be revisited after primary-user interviews.

---

# 3. Researcher Workflow

## Example information need

> "How has rainfall changed across a particular region of Kenya over the past 20 years, and which areas have experienced persistent anomalies?"

## Current working workflow

```text
Research question
       ↓
Define geographic area
       ↓
Identify required variables
       ↓
Search for datasets
       ↓
Compare possible sources
       ↓
Check methodology / resolution / coverage
       ↓
Download data
       ↓
Clean / extract
       ↓
Clip to study area
       ↓
Reproject / convert if necessary
       ↓
Aggregate / calculate indicators
       ↓
Combine with boundaries or other datasets
       ↓
Analyse
       ↓
Create maps / charts
       ↓
Interpret results
       ↓
Write report / paper
```

## Possible sources

* Kenya Meteorological Department
* ICPAC
* World Bank Climate Change Knowledge Portal
* Copernicus Climate Data Store
* CHIRPS
* NASA
* other research datasets

## Possible tools

* QGIS
* ArcGIS
* Python
* R
* Excel
* SQL
* visualization/reporting tools

## Potential friction to investigate

### Discovery

* Difficulty determining which dataset is appropriate
* Multiple possible sources
* Different terminology between providers

### Access

* Different access mechanisms
* Registration or formal requests
* Different download mechanisms
* API requirements

### Processing

* Data extraction
* Format conversion
* Clipping
* Reprojection
* Aggregation
* Raster/vector processing

### Integration

* Combining climate data with administrative boundaries
* Combining datasets with different spatial/temporal resolutions
* Combining multiple providers

### Analysis

* Technical knowledge requirements
* Need for multiple software tools

### Communication

* Producing publication-ready maps and charts
* Converting analysis into reports

These are hypotheses to validate.

---

# 4. NGO / Humanitarian / Development Workflow

This workflow is particularly important because this is currently the project's provisional primary user segment.

Unlike a researcher, the user's starting point may be a **programme or operational question** rather than a climate-data question.

## Example information need

> "Which of our programme areas are experiencing drought conditions, and what might this mean for planned activities?"

## Current working workflow

```text
Programme / operational question
             ↓
Identify geographic areas
             ↓
Identify relevant climate hazard
             ↓
Find climate information
             ↓
Find contextual information
             ↓
Access multiple sources
             ↓
Download / extract data
             ↓
Clean / standardize
             ↓
Combine climate + programme data
             ↓
GIS / analysis
             ↓
Interpret
             ↓
Create map / dashboard / briefing
             ↓
Share with programme / management team
             ↓
Decision / action
```

---

## Possible information inputs

### Climate

* rainfall
* drought indicators
* temperature
* floods
* forecasts
* seasonal climate information

### Humanitarian/development

* population
* vulnerability
* food security
* programme locations
* infrastructure
* administrative boundaries
* affected populations
* organizational presence

### Environmental

* vegetation
* soil moisture
* land cover
* satellite imagery
* environmental indicators

---

## Possible sources

* KMD
* ICPAC
* NDMA
* RCMRD
* HDX
* OCHA information products
* satellite/Earth-observation sources
* organization-specific datasets

---

## Possible tools

| Task                | Possible tool                                      |
| ------------------- | -------------------------------------------------- |
| Climate information | KMD / ICPAC / other sources                        |
| Humanitarian data   | HDX / OCHA                                         |
| Field data          | KoboToolbox                                        |
| GIS                 | QGIS / ArcGIS                                      |
| Analysis            | Excel / Python / R                                 |
| Dashboard           | Power BI / GIS dashboards                          |
| Reporting           | PowerPoint / Word / PDF                            |
| Collaboration       | SharePoint / Google Drive / organizational systems |

---

## Potential friction to investigate

### Fragmentation

Climate information may be located separately from programme data.

### Technical dependency

Programme staff may depend on GIS/data specialists for processing.

### Repeated processing

The same datasets may need to be downloaded, cleaned and prepared repeatedly.

### Timing

Information may not be available in the format or timeframe required for a decision.

### Contextualization

Users may need to combine climate indicators with operational information.

### Interpretation

A climate indicator may not directly answer:

> "What does this mean for our programme?"

These are hypotheses requiring interviews.

---

# 5. Developer / Data Professional Workflow

## Example information need

> "I want to build an application displaying rainfall conditions for Kenyan counties."

## Current working workflow

```text
Application requirement
        ↓
Determine required climate variable
        ↓
Search for data / API
        ↓
Compare providers
        ↓
Check documentation
        ↓
Check licensing
        ↓
Create account / credentials
        ↓
Test API
        ↓
Retrieve data
        ↓
Parse / transform
        ↓
Store in database
        ↓
Build application
        ↓
Monitor API / data reliability
        ↓
Handle updates / errors
```

---

## Possible technical requirements

* API access
* authentication
* documentation
* machine-readable formats
* historical data
* geographic filtering
* metadata
* update frequency
* licensing
* reliability
* rate limits

---

## Possible tools

* Python
* JavaScript
* SQL
* REST APIs
* GIS libraries
* PostgreSQL/PostGIS
* cloud/database infrastructure
* visualization libraries

---

## Potential technical friction

| Potential issue         | Why it could matter                       |
| ----------------------- | ----------------------------------------- |
| Poor documentation      | Increases development time                |
| Authentication          | Adds implementation work                  |
| Different formats       | Requires transformation                   |
| Inconsistent schemas    | Complicates integration                   |
| API limits              | Can affect scaling                        |
| Large datasets          | Increases storage/processing requirements |
| Licensing uncertainty   | Creates commercial risk                   |
| Data updates            | Requires monitoring                       |
| Missing historical data | Limits applications                       |
| Unreliable endpoints    | Creates production risk                   |

These are hypotheses and must be validated with developers/data professionals.

---

# 6. Cross-User Workflow

Across all three user types, a generalized workflow can be represented as:

```text
                CLIMATE / WEATHER QUESTION
                           ↓
                  FIND INFORMATION
                           ↓
          ┌────────────────┼────────────────┐
          ↓                ↓                ↓
      Researcher          NGO           Developer
          ↓                ↓                ↓
      Compare          Find context     Check API
      datasets        + programme          ↓
          ↓                ↓             Retrieve
       Download         Download            ↓
          ↓                ↓             Process
          └────────────────┼────────────────┘
                           ↓
                   PROCESS / TRANSFORM
                           ↓
                    COMBINE DATA
                           ↓
                       ANALYSE
                           ↓
                 VISUALIZE / COMMUNICATE
                           ↓
                       USE RESULT
```

This represents a conceptual workflow rather than a universal process.

---

# 7. Data Handoffs

A major area to investigate is the movement of information between platforms and tools.

## Example 1 — Research

```text
ICPAC
  ↓
Download climate dataset
  ↓
QGIS
  ↓
Administrative boundaries
  ↓
Python / R
  ↓
Statistical analysis
  ↓
Maps / charts
  ↓
Research paper
```

## Example 2 — NGO / Humanitarian

```text
Climate information provider
          ↓
Climate dataset
          ↓
GIS specialist
          ↓
Programme dataset
          ↓
GIS analysis
          ↓
Dashboard / map
          ↓
Programme manager
          ↓
Decision
```

## Example 3 — Developer

```text
Climate API
     ↓
Application code
     ↓
Data transformation
     ↓
Database
     ↓
Web application
     ↓
End user
```

Each transition between systems is a **handoff**.

Potential problems associated with handoffs include:

* duplicated work;
* incompatible formats;
* inconsistent schemas;
* delays;
* errors;
* loss of context;
* dependency on technical staff.

Whether these are significant problems must be established through interviews.

---

# 8. Workflow Friction Matrix

The following matrix is intentionally left open for evidence from interviews.

| Workflow stage          | Researcher  | NGO / Humanitarian | Developer   | Evidence |
| ----------------------- | ----------- | ------------------ | ----------- | -------- |
| Define information need | To validate | To validate        | To validate |          |
| Discover data           | To validate | To validate        | To validate |          |
| Compare sources         | To validate | To validate        | To validate |          |
| Access data             | To validate | To validate        | To validate |          |
| Understand metadata     | To validate | To validate        | To validate |          |
| Download                | To validate | To validate        | To validate |          |
| Clean                   | To validate | To validate        | To validate |          |
| Transform               | To validate | To validate        | To validate |          |
| Combine datasets        | To validate | To validate        | To validate |          |
| Analyse                 | To validate | To validate        | To validate |          |
| Visualize               | To validate | To validate        | To validate |          |
| Communicate             | To validate | To validate        | To validate |          |
| Make/use decision       | To validate | To validate        | To validate |          |

---

# 9. Three Types of Potential Friction

## 9.1 Discovery friction

The user has difficulty finding the right information.

Potential examples:

* too many providers;
* unclear terminology;
* difficulty comparing datasets;
* insufficient search/discovery tools;
* uncertainty about which source is appropriate.

---

## 9.2 Technical friction

The user has found the data but has difficulty using it.

Potential examples:

* API complexity;
* GIS processing;
* format conversion;
* data cleaning;
* inconsistent schemas;
* large files;
* technical requirements.

---

## 9.3 Decision friction

The user has the data but still cannot easily answer the question they care about.

Potential examples:

* need to combine multiple indicators;
* insufficient context;
* difficulty interpreting climate indicators;
* manual report/map creation;
* difficulty connecting climate information to operational decisions.

This category is particularly important for the NGO/humanitarian/development research.

---

# 10. Current Product Hypotheses

The workflow research suggests several hypotheses.

These are **not product decisions**.

## Hypothesis 1 — Discovery

Users may benefit from a unified way to discover relevant climate datasets from multiple providers.

## Hypothesis 2 — Integration

Users may benefit from combining climate information with contextual geospatial and programme data.

## Hypothesis 3 — Processing

Users may benefit from tools that reduce repetitive data preparation and GIS processing.

## Hypothesis 4 — Decision support

Users may value information presented around a specific decision or use case rather than raw datasets.

## Hypothesis 5 — Kenya-first

A Kenya-focused initial product may be more useful and manageable than immediately attempting to cover the entire African continent.

These hypotheses require validation.

---

# 11. What We Should Not Build Yet

Based on the current ecosystem research, the project should not yet assume that it needs to build:

* a new weather forecasting system;
* a replacement for KMD;
* a replacement for ICPAC;
* a replacement for Copernicus;
* a new global climate-data infrastructure;
* a generic GIS application;
* a generic dashboard builder;
* a replacement for HDX;
* a giant Africa-wide data warehouse.

Existing organizations and platforms already provide substantial functionality in these areas.

The research should instead determine whether an unmet need exists **between existing information providers and the people who need to use the information**.

---

# 12. Interview Questions Generated From the Workflow

## Discovery

1. When you need climate or weather information, where do you normally start looking?
2. Which platforms or sources do you use most?
3. How do you decide which dataset or source to use?

## Access

4. Once you identify the data, what do you have to do to obtain it?
5. Are there any access restrictions or technical requirements?

## Processing

6. What happens after you download or obtain the data?
7. Do you normally have to clean, convert, clip or otherwise process it?

## Integration

8. Do you combine climate information with other datasets?
9. What other datasets do you normally combine it with?
10. How do you perform that integration?

## Tools

11. Which software do you use?
12. Who normally performs the technical processing?

## Time

13. Which part of the process takes the most time?

## Friction

14. What is the most difficult or frustrating part of obtaining and using the information?

## Workarounds

15. What do you do when the information is not available in the format you need?

## Decision-making

16. What happens with the information after you analyse it?
17. Who uses the final output?
18. What decisions does it support?

## Improvement

19. If you could change one part of the current process, what would you change?

The improvement question should generally be asked **after** understanding the existing workflow so that the interview does not prematurely steer the participant toward our proposed solution.

---

# 13. Evidence Classification

All findings should eventually be classified as one of the following:

### Documented fact

Information supported by an official platform, dataset, publication or other reliable source.

### User-reported behaviour

Information directly reported by an interview participant.

### Observed workflow

A workflow documented by observing a user performing a task.

### Research hypothesis

An interpretation that has not yet been sufficiently validated.

### Product hypothesis

A possible solution that requires further validation.

This distinction will be maintained throughout the research.

---

# 14. Primary Research Plan

The current target is approximately:

* 2–3 researchers;
* 3–5 NGO/humanitarian/development professionals;
* 2–3 GIS/data professionals or developers.

An initial sample of approximately **7–10 useful interviews** should provide enough information to identify recurring workflow patterns for this early-stage research.

The sample can be expanded if interviews continue producing substantially different perspectives.

---

# 15. Interview Evidence Log

Each interview should eventually be recorded using the following structure:

| Field                | Information |
| -------------------- | ----------- |
| Participant ID       |             |
| User group           |             |
| Role                 |             |
| Organization type    |             |
| Date                 |             |
| Primary task         |             |
| Information required |             |
| Sources used         |             |
| Tools used           |             |
| Workflow             |             |
| Difficulties         |             |
| Workarounds          |             |
| Time/effort          |             |
| Desired improvement  |             |
| Evidence/quote       |             |
| Our interpretation   |             |
| Follow-up required   |             |

Do not record confidential organizational information unless there is an appropriate reason and permission to do so.

---

# 16. Day 11 Conclusion

The current research suggests that the climate-information ecosystem is not simply a problem of missing data.

Existing systems already provide substantial:

* observations;
* forecasts;
* climate datasets;
* environmental information;
* APIs;
* maps;
* dashboards;
* humanitarian datasets;
* geospatial information.

The more important research question is:

> **How much effort does a user have to undertake to move from existing climate information to a useful research, humanitarian, development or operational decision?**

The potential opportunity may therefore exist in the workflow between:

```text
EXISTING INFORMATION
        ↓
DISCOVERY
        ↓
ACCESS
        ↓
INTEGRATION
        ↓
PROCESSING
        ↓
ANALYSIS
        ↓
CONTEXT
        ↓
DECISION
```

The next stage is to determine which parts of this workflow actually cause problems for real users.

---

## 17. Next Step

**Day 12 — Identify and prioritize potential friction points.**

Day 12 will take the hypotheses from this document and create a **problem/friction matrix** that separates:

* evidence we already have;
* assumptions;
* questions for interviews;
* potential high-value problems;
* problems we should deliberately ignore.

# User Workflows

## Africa Climate Intelligence

**Research stage:** Week 2 — Competitor and ecosystem research
**Day:** Day 11 — Current user workflows
**Status:** Working analysis — requires primary-user validation

---

## 1. Purpose

This document maps how potential users may currently move from a climate/weather information need to a useful output.

The purpose is to understand:

* where users obtain information;
* which platforms they use;
* what tools they use;
* how datasets move between systems;
* where manual work occurs;
* where users depend on technical specialists;
* where information may be difficult to interpret or apply;
* which potential friction points should be tested through interviews.

The workflows in this document are **working hypotheses** based on ecosystem and platform research. They should not be treated as confirmed descriptions of every user's workflow.

---

# 2. Target User Groups

The current research focuses on three user groups:

1. **Researcher**
2. **NGO / humanitarian / development professional**
3. **Developer / data professional**

The NGO/humanitarian/development group remains the project's **provisional primary user segment**.

This classification will be revisited after primary-user interviews.

---

# 3. Researcher Workflow

## Example information need

> "How has rainfall changed across a particular region of Kenya over the past 20 years, and which areas have experienced persistent anomalies?"

## Current working workflow

```text
Research question
       ↓
Define geographic area
       ↓
Identify required variables
       ↓
Search for datasets
       ↓
Compare possible sources
       ↓
Check methodology / resolution / coverage
       ↓
Download data
       ↓
Clean / extract
       ↓
Clip to study area
       ↓
Reproject / convert if necessary
       ↓
Aggregate / calculate indicators
       ↓
Combine with boundaries or other datasets
       ↓
Analyse
       ↓
Create maps / charts
       ↓
Interpret results
       ↓
Write report / paper
```

## Possible sources

* Kenya Meteorological Department
* ICPAC
* World Bank Climate Change Knowledge Portal
* Copernicus Climate Data Store
* CHIRPS
* NASA
* other research datasets

## Possible tools

* QGIS
* ArcGIS
* Python
* R
* Excel
* SQL
* visualization/reporting tools

## Potential friction to investigate

### Discovery

* Difficulty determining which dataset is appropriate
* Multiple possible sources
* Different terminology between providers

### Access

* Different access mechanisms
* Registration or formal requests
* Different download mechanisms
* API requirements

### Processing

* Data extraction
* Format conversion
* Clipping
* Reprojection
* Aggregation
* Raster/vector processing

### Integration

* Combining climate data with administrative boundaries
* Combining datasets with different spatial/temporal resolutions
* Combining multiple providers

### Analysis

* Technical knowledge requirements
* Need for multiple software tools

### Communication

* Producing publication-ready maps and charts
* Converting analysis into reports

These are hypotheses to validate.

---

# 4. NGO / Humanitarian / Development Workflow

This workflow is particularly important because this is currently the project's provisional primary user segment.

Unlike a researcher, the user's starting point may be a **programme or operational question** rather than a climate-data question.

## Example information need

> "Which of our programme areas are experiencing drought conditions, and what might this mean for planned activities?"

## Current working workflow

```text
Programme / operational question
             ↓
Identify geographic areas
             ↓
Identify relevant climate hazard
             ↓
Find climate information
             ↓
Find contextual information
             ↓
Access multiple sources
             ↓
Download / extract data
             ↓
Clean / standardize
             ↓
Combine climate + programme data
             ↓
GIS / analysis
             ↓
Interpret
             ↓
Create map / dashboard / briefing
             ↓
Share with programme / management team
             ↓
Decision / action
```

---

## Possible information inputs

### Climate

* rainfall
* drought indicators
* temperature
* floods
* forecasts
* seasonal climate information

### Humanitarian/development

* population
* vulnerability
* food security
* programme locations
* infrastructure
* administrative boundaries
* affected populations
* organizational presence

### Environmental

* vegetation
* soil moisture
* land cover
* satellite imagery
* environmental indicators

---

## Possible sources

* KMD
* ICPAC
* NDMA
* RCMRD
* HDX
* OCHA information products
* satellite/Earth-observation sources
* organization-specific datasets

---

## Possible tools

| Task                | Possible tool                                      |
| ------------------- | -------------------------------------------------- |
| Climate information | KMD / ICPAC / other sources                        |
| Humanitarian data   | HDX / OCHA                                         |
| Field data          | KoboToolbox                                        |
| GIS                 | QGIS / ArcGIS                                      |
| Analysis            | Excel / Python / R                                 |
| Dashboard           | Power BI / GIS dashboards                          |
| Reporting           | PowerPoint / Word / PDF                            |
| Collaboration       | SharePoint / Google Drive / organizational systems |

---

## Potential friction to investigate

### Fragmentation

Climate information may be located separately from programme data.

### Technical dependency

Programme staff may depend on GIS/data specialists for processing.

### Repeated processing

The same datasets may need to be downloaded, cleaned and prepared repeatedly.

### Timing

Information may not be available in the format or timeframe required for a decision.

### Contextualization

Users may need to combine climate indicators with operational information.

### Interpretation

A climate indicator may not directly answer:

> "What does this mean for our programme?"

These are hypotheses requiring interviews.

---

# 5. Developer / Data Professional Workflow

## Example information need

> "I want to build an application displaying rainfall conditions for Kenyan counties."

## Current working workflow

```text
Application requirement
        ↓
Determine required climate variable
        ↓
Search for data / API
        ↓
Compare providers
        ↓
Check documentation
        ↓
Check licensing
        ↓
Create account / credentials
        ↓
Test API
        ↓
Retrieve data
        ↓
Parse / transform
        ↓
Store in database
        ↓
Build application
        ↓
Monitor API / data reliability
        ↓
Handle updates / errors
```

---

## Possible technical requirements

* API access
* authentication
* documentation
* machine-readable formats
* historical data
* geographic filtering
* metadata
* update frequency
* licensing
* reliability
* rate limits

---

## Possible tools

* Python
* JavaScript
* SQL
* REST APIs
* GIS libraries
* PostgreSQL/PostGIS
* cloud/database infrastructure
* visualization libraries

---

## Potential technical friction

| Potential issue         | Why it could matter                       |
| ----------------------- | ----------------------------------------- |
| Poor documentation      | Increases development time                |
| Authentication          | Adds implementation work                  |
| Different formats       | Requires transformation                   |
| Inconsistent schemas    | Complicates integration                   |
| API limits              | Can affect scaling                        |
| Large datasets          | Increases storage/processing requirements |
| Licensing uncertainty   | Creates commercial risk                   |
| Data updates            | Requires monitoring                       |
| Missing historical data | Limits applications                       |
| Unreliable endpoints    | Creates production risk                   |

These are hypotheses and must be validated with developers/data professionals.

---

# 6. Cross-User Workflow

Across all three user types, a generalized workflow can be represented as:

```text
                CLIMATE / WEATHER QUESTION
                           ↓
                  FIND INFORMATION
                           ↓
          ┌────────────────┼────────────────┐
          ↓                ↓                ↓
      Researcher          NGO           Developer
          ↓                ↓                ↓
      Compare          Find context     Check API
      datasets        + programme          ↓
          ↓                ↓             Retrieve
       Download         Download            ↓
          ↓                ↓             Process
          └────────────────┼────────────────┘
                           ↓
                   PROCESS / TRANSFORM
                           ↓
                    COMBINE DATA
                           ↓
                       ANALYSE
                           ↓
                 VISUALIZE / COMMUNICATE
                           ↓
                       USE RESULT
```

This represents a conceptual workflow rather than a universal process.

---

# 7. Data Handoffs

A major area to investigate is the movement of information between platforms and tools.

## Example 1 — Research

```text
ICPAC
  ↓
Download climate dataset
  ↓
QGIS
  ↓
Administrative boundaries
  ↓
Python / R
  ↓
Statistical analysis
  ↓
Maps / charts
  ↓
Research paper
```

## Example 2 — NGO / Humanitarian

```text
Climate information provider
          ↓
Climate dataset
          ↓
GIS specialist
          ↓
Programme dataset
          ↓
GIS analysis
          ↓
Dashboard / map
          ↓
Programme manager
          ↓
Decision
```

## Example 3 — Developer

```text
Climate API
     ↓
Application code
     ↓
Data transformation
     ↓
Database
     ↓
Web application
     ↓
End user
```

Each transition between systems is a **handoff**.

Potential problems associated with handoffs include:

* duplicated work;
* incompatible formats;
* inconsistent schemas;
* delays;
* errors;
* loss of context;
* dependency on technical staff.

Whether these are significant problems must be established through interviews.

---

# 8. Workflow Friction Matrix

The following matrix is intentionally left open for evidence from interviews.

| Workflow stage          | Researcher  | NGO / Humanitarian | Developer   | Evidence |
| ----------------------- | ----------- | ------------------ | ----------- | -------- |
| Define information need | To validate | To validate        | To validate |          |
| Discover data           | To validate | To validate        | To validate |          |
| Compare sources         | To validate | To validate        | To validate |          |
| Access data             | To validate | To validate        | To validate |          |
| Understand metadata     | To validate | To validate        | To validate |          |
| Download                | To validate | To validate        | To validate |          |
| Clean                   | To validate | To validate        | To validate |          |
| Transform               | To validate | To validate        | To validate |          |
| Combine datasets        | To validate | To validate        | To validate |          |
| Analyse                 | To validate | To validate        | To validate |          |
| Visualize               | To validate | To validate        | To validate |          |
| Communicate             | To validate | To validate        | To validate |          |
| Make/use decision       | To validate | To validate        | To validate |          |

---

# 9. Three Types of Potential Friction

## 9.1 Discovery friction

The user has difficulty finding the right information.

Potential examples:

* too many providers;
* unclear terminology;
* difficulty comparing datasets;
* insufficient search/discovery tools;
* uncertainty about which source is appropriate.

---

## 9.2 Technical friction

The user has found the data but has difficulty using it.

Potential examples:

* API complexity;
* GIS processing;
* format conversion;
* data cleaning;
* inconsistent schemas;
* large files;
* technical requirements.

---

## 9.3 Decision friction

The user has the data but still cannot easily answer the question they care about.

Potential examples:

* need to combine multiple indicators;
* insufficient context;
* difficulty interpreting climate indicators;
* manual report/map creation;
* difficulty connecting climate information to operational decisions.

This category is particularly important for the NGO/humanitarian/development research.

---

# 10. Current Product Hypotheses

The workflow research suggests several hypotheses.

These are **not product decisions**.

## Hypothesis 1 — Discovery

Users may benefit from a unified way to discover relevant climate datasets from multiple providers.

## Hypothesis 2 — Integration

Users may benefit from combining climate information with contextual geospatial and programme data.

## Hypothesis 3 — Processing

Users may benefit from tools that reduce repetitive data preparation and GIS processing.

## Hypothesis 4 — Decision support

Users may value information presented around a specific decision or use case rather than raw datasets.

## Hypothesis 5 — Kenya-first

A Kenya-focused initial product may be more useful and manageable than immediately attempting to cover the entire African continent.

These hypotheses require validation.

---

# 11. What We Should Not Build Yet

Based on the current ecosystem research, the project should not yet assume that it needs to build:

* a new weather forecasting system;
* a replacement for KMD;
* a replacement for ICPAC;
* a replacement for Copernicus;
* a new global climate-data infrastructure;
* a generic GIS application;
* a generic dashboard builder;
* a replacement for HDX;
* a giant Africa-wide data warehouse.

Existing organizations and platforms already provide substantial functionality in these areas.

The research should instead determine whether an unmet need exists **between existing information providers and the people who need to use the information**.

---

# 12. Interview Questions Generated From the Workflow

## Discovery

1. When you need climate or weather information, where do you normally start looking?
2. Which platforms or sources do you use most?
3. How do you decide which dataset or source to use?

## Access

4. Once you identify the data, what do you have to do to obtain it?
5. Are there any access restrictions or technical requirements?

## Processing

6. What happens after you download or obtain the data?
7. Do you normally have to clean, convert, clip or otherwise process it?

## Integration

8. Do you combine climate information with other datasets?
9. What other datasets do you normally combine it with?
10. How do you perform that integration?

## Tools

11. Which software do you use?
12. Who normally performs the technical processing?

## Time

13. Which part of the process takes the most time?

## Friction

14. What is the most difficult or frustrating part of obtaining and using the information?

## Workarounds

15. What do you do when the information is not available in the format you need?

## Decision-making

16. What happens with the information after you analyse it?
17. Who uses the final output?
18. What decisions does it support?

## Improvement

19. If you could change one part of the current process, what would you change?

The improvement question should generally be asked **after** understanding the existing workflow so that the interview does not prematurely steer the participant toward our proposed solution.

---

# 13. Evidence Classification

All findings should eventually be classified as one of the following:

### Documented fact

Information supported by an official platform, dataset, publication or other reliable source.

### User-reported behaviour

Information directly reported by an interview participant.

### Observed workflow

A workflow documented by observing a user performing a task.

### Research hypothesis

An interpretation that has not yet been sufficiently validated.

### Product hypothesis

A possible solution that requires further validation.

This distinction will be maintained throughout the research.

---

# 14. Primary Research Plan

The current target is approximately:

* 2–3 researchers;
* 3–5 NGO/humanitarian/development professionals;
* 2–3 GIS/data professionals or developers.

An initial sample of approximately **7–10 useful interviews** should provide enough information to identify recurring workflow patterns for this early-stage research.

The sample can be expanded if interviews continue producing substantially different perspectives.

---

# 15. Interview Evidence Log

Each interview should eventually be recorded using the following structure:

| Field                | Information |
| -------------------- | ----------- |
| Participant ID       |             |
| User group           |             |
| Role                 |             |
| Organization type    |             |
| Date                 |             |
| Primary task         |             |
| Information required |             |
| Sources used         |             |
| Tools used           |             |
| Workflow             |             |
| Difficulties         |             |
| Workarounds          |             |
| Time/effort          |             |
| Desired improvement  |             |
| Evidence/quote       |             |
| Our interpretation   |             |
| Follow-up required   |             |

Do not record confidential organizational information unless there is an appropriate reason and permission to do so.

---

# 16. Day 11 Conclusion

The current research suggests that the climate-information ecosystem is not simply a problem of missing data.

Existing systems already provide substantial:

* observations;
* forecasts;
* climate datasets;
* environmental information;
* APIs;
* maps;
* dashboards;
* humanitarian datasets;
* geospatial information.

The more important research question is:

> **How much effort does a user have to undertake to move from existing climate information to a useful research, humanitarian, development or operational decision?**

The potential opportunity may therefore exist in the workflow between:

```text
EXISTING INFORMATION
        ↓
DISCOVERY
        ↓
ACCESS
        ↓
INTEGRATION
        ↓
PROCESSING
        ↓
ANALYSIS
        ↓
CONTEXT
        ↓
DECISION
```

The next stage is to determine which parts of this workflow actually cause problems for real users.

---

## 17. Next Step

**Day 12 — Identify and prioritize potential friction points.**

Day 12 will take the hypotheses from this document and create a **problem/friction matrix** that separates:

* evidence we already have;
* assumptions;
* questions for interviews;
* potential high-value problems;
* problems we should deliberately ignore.

This will prepare the project for **primary-user interviews in Week 3**.


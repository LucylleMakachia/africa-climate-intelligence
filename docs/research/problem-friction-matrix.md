# Problem & Friction Matrix

## Africa Climate Intelligence

**Research stage:** Week 2 — Competitor and ecosystem research
**Day:** Day 12 — Identify and prioritize workflow friction
**Geographic focus:** Kenya
**Primary user segment:** NGOs / humanitarian / development organizations
**Secondary users:** Researchers and developers/data professionals
**Status:** Working hypotheses — primary-user validation required

---

# 1. Purpose

This document identifies potential problems and friction points that
users may experience when finding, accessing, processing, combining and
using climate/weather information.

The findings are based on:

* ecosystem mapping;
* existing-platform research;
* user-workflow analysis;
* the project's initial target users and use cases.

The purpose is to determine which issues should be investigated during
user interviews.

This document does **not** establish that these problems definitely
exist.

The distinction between evidence and assumptions is maintained
throughout the research.

---

# 2. Evidence Classification

| Classification                        | Meaning                                                                |
| ------------------------------------- | ---------------------------------------------------------------------- |
| **Documented fact**                   | Supported by existing platform, institutional or dataset documentation |
| **Observed ecosystem characteristic** | A characteristic identified through platform/ecosystem research        |
| **Hypothesis**                        | A possible user problem inferred from the research                     |
| **User-reported**                     | Directly reported by an interview participant                          |
| **Validated problem**                 | Repeatedly supported by independent user evidence                      |
| **Product hypothesis**                | A possible solution to a validated problem                             |

At the current stage, most findings in this document are **hypotheses**.

---

# 3. Overall Finding

The research conducted during Week 2 suggests that Kenya and the wider
East African climate-information ecosystem already contains substantial
data, platforms and technical infrastructure.

Relevant information is available through organizations and systems
including:

* Kenya Meteorological Department;
* ICPAC;
* World Bank Climate Change Knowledge Portal;
* Copernicus;
* HDX;
* Earth-observation providers;
* humanitarian information systems;
* organizational/project datasets.

Therefore, the project's initial problem should **not** simply be:

> "Climate data is unavailable."

A more useful working hypothesis is:

> **Climate and weather information relevant to Kenya is available
> through multiple national, regional and global sources, but users may
> still experience difficulty discovering appropriate datasets,
> accessing them, preparing and combining them with contextual
> information, and turning them into useful research, humanitarian,
> development or operational outputs.**

This statement requires validation through primary research.

---

# 4. Potential Friction Areas

## 4.1 Data Discovery

### Potential problem

Users may have difficulty identifying the most appropriate climate or
weather dataset for a particular task.

There are multiple possible sources, including national, regional and
global providers.

### Potential users

* Researchers
* NGOs
* Humanitarian organizations
* Development organizations
* Developers

### Possible causes

* multiple providers;
* different datasets;
* different terminology;
* different spatial/temporal resolutions;
* uncertainty about which dataset is appropriate.

### Possible consequence

Users may spend additional time searching, comparing and evaluating
datasets before beginning their actual analysis.

### Evidence status

**Hypothesis**

### Interview validation

Ask:

> "When you need climate or weather information, where do you normally
> start looking?"

> "How do you decide which dataset to use?"

---

# 5. Data Fragmentation

## Potential problem

Relevant information may be distributed across multiple platforms.

For example:

```text
KMD
 ↓
ICPAC
 ↓
Copernicus
 ↓
HDX
 ↓
Earth-observation sources
 ↓
Organization's own datasets
```

A user may need information from several of these sources for one
analysis.

### Potential users

Particularly:

* NGOs;
* humanitarian organizations;
* researchers.

### Potential consequence

Users may need to:

* visit multiple platforms;
* learn different interfaces;
* download multiple datasets;
* reconcile different formats;
* manually combine information.

### Evidence status

**Observed ecosystem characteristic → user problem still requires
validation**

### Interview validation

> "For the last climate-related analysis you conducted, how many
> different data sources did you use?"

---

# 6. Different Data-Access Mechanisms

## Potential problem

Climate information can be accessed through different mechanisms,
depending on the provider and dataset.

Examples include:

* web portals;
* downloads;
* APIs;
* registration;
* formal data requests;
* machine-readable datasets.

### Potential users

All three target groups.

### Potential consequence

Users may have to understand different procedures for different sources.

Developers may also have to implement multiple APIs.

### Evidence status

**Documented ecosystem characteristic**

Whether this creates significant user friction is **unvalidated**.

### Interview validation

> "Have you ever found the data you need but struggled to actually
> obtain it?"

---

# 7. Repetitive Data Preparation

## Potential problem

Users may repeatedly need to prepare climate data before it can be
used.

Potential operations include:

```text
Download
 ↓
Extract
 ↓
Clean
 ↓
Clip
 ↓
Reproject
 ↓
Convert
 ↓
Aggregate
 ↓
Join
```

### Potential users

* Researchers
* GIS analysts
* NGOs
* Humanitarian organizations
* Developers

### Potential consequence

Additional:

* staff time;
* technical effort;
* processing;
* opportunities for errors.

### Evidence status

**Hypothesis**

### Interview validation

> "After you obtain the data, what do you normally have to do before
> you can actually use it?"

---

# 8. Combining Climate and Contextual Data

## Potential problem

Users may need to combine climate information with other information
to answer their actual question.

For example:

```text
Rainfall
    +
Population
    +
Programme locations
    +
Administrative boundaries
    +
Vulnerability
    ↓
Climate-risk analysis
```

### Potential users

Especially:

* NGOs;
* humanitarian organizations;
* development organizations.

### Why this matters

A climate dataset by itself may not answer the operational question.

The user may actually need to know:

> "Which people, assets or programmes are potentially affected?"

### Potential consequence

Users may have to obtain, clean and integrate several independent
datasets.

### Evidence status

**High-priority hypothesis**

### Interview validation

> "Do you normally combine climate information with other datasets?"

> "What other datasets do you combine it with?"

> "How do you perform that integration?"

---

# 9. Technical Dependency

## Potential problem

Non-technical programme staff may depend on GIS, data or IT specialists
to obtain and process climate information.

Possible workflow:

```text
Programme Officer
       ↓
Needs information
       ↓
Requests GIS/Data team
       ↓
Analyst searches for data
       ↓
Analyst processes data
       ↓
Analyst produces map
       ↓
Programme officer receives result
```

### Potential users

* Programme staff;
* humanitarian practitioners;
* development practitioners.

### Potential consequence

The person with the operational question may not be able to obtain
the answer independently.

### Important caution

This is **not automatically a problem**.

Technical specialization may be an intentional and effective
organizational structure.

### Evidence status

**Hypothesis**

### Interview validation

> "Who normally obtains and analyses climate information in your
> organization?"

> "What happens if that person is unavailable?"

---

# 10. Time from Question to Answer

## Potential problem

The complete process from identifying an information need to producing
a usable answer may take substantial time.

The actual duration is currently unknown.

### Potential users

All three groups.

### Why this matters

Time is potentially more useful to measure than whether a user simply
describes a system as "difficult."

### Key metric

```text
Time from:
"I need this information"
        ↓
"I have a usable answer"
```

### Evidence status

**Major evidence gap**

### Interview validation

> "Think about the last time you needed climate information. How long
> did it take from starting the search to producing something you could
> actually use?"

> "Which step took the longest?"

---

# 11. Repeated Manual Work

## Potential problem

Users or organizations may repeatedly perform similar data-processing
tasks.

Example:

```text
Every month:
    ↓
Find dataset
    ↓
Download
    ↓
Clean
    ↓
Clip
    ↓
Analyse
    ↓
Create map
    ↓
Prepare report
```

### Why it matters

A task performed once may not justify automation.

A task performed every week or month could represent significant
cumulative effort.

### Evidence status

**Major hypothesis requiring validation**

### Interview validation

> "How often do you perform this type of analysis?"

> "Do you repeat the same data-preparation steps?"

---

# 12. Data Interpretation

## Potential problem

Users may have access to climate indicators but still need help
understanding what those indicators mean for their particular
question.

Example:

```text
Climate indicator
       ↓
Analysis
       ↓
Context
       ↓
Operational meaning
```

A raw rainfall anomaly does not necessarily answer:

> "What does this mean for our programme?"

### Potential users

Especially:

* NGOs;
* humanitarian organizations;
* development organizations;
* programme managers.

### Evidence status

**High-priority hypothesis**

### Interview validation

> "Once you have the climate information, how do you turn it into
> something useful for a programme or decision?"

---

# 13. Dataset Selection and Trust

## Potential problem

Users may encounter multiple datasets describing similar phenomena.

They may need to compare:

* source;
* methodology;
* resolution;
* temporal coverage;
* update frequency;
* accuracy/quality information;
* licensing;
* intended use.

### Potential users

* Researchers
* NGOs
* Developers

### Potential consequence

Users may spend time determining whether a dataset is appropriate and
credible.

### Evidence status

**Hypothesis**

### Interview validation

> "What makes you trust one climate dataset over another?"

> "Have you ever rejected a dataset because you couldn't establish
> whether it was appropriate?"

---

# 14. Data Interoperability

## Potential problem

Different datasets may use different:

* file formats;
* coordinate systems;
* geographic identifiers;
* spatial resolutions;
* temporal resolutions;
* schemas.

Example:

```text
Dataset A → GeoTIFF
Dataset B → CSV
Dataset C → NetCDF
Dataset D → JSON/API
Dataset E → Excel
```

### Potential users

Especially:

* researchers;
* GIS professionals;
* developers.

### Potential consequence

Additional conversion and transformation work.

### Evidence status

**Hypothesis**

### Interview validation

> "Have you encountered problems combining climate datasets from
> different providers?"

---

# 15. Developer/API Friction

## Potential problem

Developers may encounter difficulty integrating climate information
into applications.

Possible issues include:

* documentation;
* authentication;
* rate limits;
* endpoint structure;
* data formats;
* historical-data availability;
* licensing;
* reliability;
* update mechanisms.

### Potential users

Developers and data professionals.

### Evidence status

**Hypothesis**

### Interview validation

> "What is the most difficult part of integrating weather or climate
> data into an application?"

---

# 16. Problem/Friction Matrix

| #  | Potential problem                                                      | Main users               | Workflow stage | Potential impact      | Evidence status                     | Interview priority |
| -- | ---------------------------------------------------------------------- | ------------------------ | -------------- | --------------------- | ----------------------------------- | ------------------ |
| 1  | Difficult dataset discovery                                            | Researchers / NGOs       | Discovery      | Medium–High           | Hypothesis                          | **High**           |
| 2  | Information fragmented across platforms                                | Researchers / NGOs       | Discovery      | High                  | Ecosystem observation               | **High**           |
| 3  | Different data-access mechanisms                                       | All                      | Access         | Medium                | Documented ecosystem characteristic | Medium             |
| 4  | Repetitive data preparation                                            | Researchers / NGOs       | Processing     | High                  | Hypothesis                          | **High**           |
| 5  | Combining climate + programme/contextual data                          | NGOs / humanitarian      | Integration    | Potentially very high | Hypothesis                          | **Very High**      |
| 6  | Raw climate information does not directly answer operational questions | NGOs / development       | Interpretation | Potentially high      | Hypothesis                          | **Very High**      |
| 7  | Dependence on technical specialists                                    | NGOs                     | Processing     | Medium–High           | Hypothesis                          | **High**           |
| 8  | Long time from information need to usable answer                       | All                      | End-to-end     | High                  | Evidence gap                        | **Very High**      |
| 9  | Repeated manual workflows                                              | NGOs / researchers       | Processing     | High                  | Evidence gap                        | **Very High**      |
| 10 | Difficulty evaluating datasets                                         | Researchers / NGOs       | Discovery      | Medium                | Hypothesis                          | Medium             |
| 11 | Interoperability problems                                              | Researchers / developers | Integration    | Medium–High           | Hypothesis                          | Medium             |
| 12 | API/integration difficulties                                           | Developers               | Access         | Medium                | Hypothesis                          | Medium             |

---

# 17. Highest-Priority Research Questions

The current evidence suggests that interviews should concentrate on
five areas.

## Priority 1 — Climate + operational/contextual data

**Question:**

> Do NGOs/humanitarian/development organizations actually need to
> combine climate information with programme, population,
> infrastructure or vulnerability data?

If yes:

* which datasets?
* how frequently?
* who performs the work?
* what tools are used?
* what problems occur?

---

## Priority 2 — Time

**Question:**

> How long does it take to go from an information need to a usable
> climate-related output?

Measure the complete workflow.

---

## Priority 3 — Repetition

**Question:**

> Which climate-data workflows are performed repeatedly?

Determine:

* frequency;
* duration;
* staff involved;
* manual steps;
* existing automation.

---

## Priority 4 — Decision relevance

**Question:**

> What does the user actually need the climate information to help
> them decide?

This prevents the project from becoming a generic data repository.

---

## Priority 5 — Existing workarounds

**Question:**

> How do users solve the problem today?

This is critical.

The current solution may be:

* internal GIS teams;
* consultants;
* spreadsheets;
* Python scripts;
* QGIS;
* ArcGIS;
* existing dashboards;
* manual reports;
* organizational databases.

The project must eventually be better than the **actual workaround**, not
merely better than another website.

---

# 18. Problems We Should Not Pursue Yet

The following should remain outside the current MVP discussion unless
research produces evidence that they are necessary.

### ❌ Build a new weather forecasting model

Existing meteorological and climate institutions already perform
forecasting.

### ❌ Replace KMD

The project should not attempt to reproduce national meteorological
services.

### ❌ Replace ICPAC

ICPAC already provides extensive regional climate services.

### ❌ Replace Copernicus

Copernicus provides major global climate-data infrastructure.

### ❌ Replace HDX

HDX already provides humanitarian data discovery and infrastructure.

### ❌ Build a generic GIS application

The project does not need to compete with QGIS or ArcGIS.

### ❌ Build a generic dashboard platform

Existing dashboard and BI tools already serve this purpose.

### ❌ Build an "everything Africa" platform immediately

Geographic expansion should follow evidence and validated use cases.

---

# 19. Current Working Opportunity

The current research suggests a potential opportunity at the intersection
of:

```text
Existing climate information
            +
Contextual / programme data
            +
GIS / data processing
            +
User-specific questions
            ↓
Decision-ready information
```

This is **not yet a product definition**.

It is a research direction to test.

---

# 20. Working Problem Statement

For the remainder of Week 2, use this as the provisional problem
statement:

> **Climate and weather information relevant to Kenya is available
> through multiple national, regional and global sources. However,
> users may still face difficulties discovering appropriate datasets,
> accessing and preparing them, combining them with contextual
> information, and translating the resulting analysis into useful
> research, humanitarian, development or operational outputs.**

The wording should be revised after interviews.

---

# 21. What Would Validate the Problem?

We should consider the problem increasingly credible if interviews
reveal recurring evidence such as:

* several independent users describe the same workflow;
* users spend significant time on the workflow;
* the workflow occurs frequently;
* users rely on manual workarounds;
* users combine multiple datasets;
* users require specialist support;
* users experience delays;
* users have already attempted to improve the process;
* organizations allocate staff/resources to the problem;
* users can clearly explain the consequences of the problem.

A single person saying:

> "That sounds annoying."

is insufficient validation.

A stronger signal would be:

> "Every month I spend several hours downloading and processing
> rainfall data, joining it to our programme locations, and producing
> maps for our programme team."

The exact wording above is an **example of the type of evidence we want
to uncover**, not a claim that a user has said it.

---

# 22. What Would Disprove or Weaken the Hypothesis?

The research should also actively look for evidence against the idea.

The hypothesis would be weakened if interviews show that:

* users already have efficient solutions;
* the workflow happens very rarely;
* users do not consider it a significant problem;
* organizations have no meaningful need for integration;
* existing platforms already solve the problem adequately;
* users prefer existing internal systems;
* the proposed problem does not affect our target users;
* there is insufficient willingness to change the existing workflow.

This is an important part of the research.

The objective is to discover whether a worthwhile problem exists, not to
prove that the project must exist.

---

# 23. Day 12 Deliverables

### Completed

* [x] Identify potential friction points
* [x] Separate facts from hypotheses
* [x] Map discovery friction
* [x] Map access friction
* [x] Map processing friction
* [x] Map integration friction
* [x] Map interpretation friction
* [x] Identify technical dependency
* [x] Identify time/repetition questions
* [x] Identify data trust/interoperability issues
* [x] Identify developer/API issues
* [x] Create problem/friction matrix
* [x] Prioritize interview questions
* [x] Establish provisional problem statement
* [x] Define evidence needed for validation
* [x] Define evidence that could weaken the hypothesis

### Still required

* [ ] Primary-user interviews
* [ ] User-reported evidence
* [ ] Workflow observations
* [ ] Frequency estimates
* [ ] Time/effort estimates
* [ ] Validation of willingness to change
* [ ] Validation of economic/value implications

---

# 24. Transition to Day 13

Day 13 will turn this research into the **actual interview research
package**.

It should produce:

```text
docs/
└── research/
    ├── interview-guide.md
    ├── interview-notes-template.md
    ├── interview-tracker.md
    └── outreach-list.md
```

The interviews will then allow us to replace:

**"Users may have this problem"**

with:

**"Users in this specific group repeatedly experience this specific
problem, under these circumstances, using these current workarounds."**

That is the evidence we need before designing the MVP.

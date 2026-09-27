# Day 14 Research Synthesis

## Africa Climate Intelligence

**Research stage:** Week 2 → Week 3 transition
**Day:** Day 14
**Geographic focus:** Kenya
**Primary user segment:** NGOs / humanitarian / development organizations
**Secondary users:** Researchers; developers / GIS / data professionals
**Status:** Working research synthesis — MVP not yet selected

---

# 1. Purpose

This document consolidates the research completed during Days 8–13.

It brings together:

* climate-information ecosystem mapping;
* provider and platform research;
* user and stakeholder mapping;
* current user workflows;
* potential workflow friction;
* opportunity gaps;
* interview preparation.

The purpose is to establish what is currently known, what remains a
hypothesis, and which questions must be answered before selecting the
MVP.

This document is a **research synthesis**, not a final product
definition.

---

# 2. Research Position

The project has now moved through three stages:

```text
WEEK 1
Problem + users + geography + initial use cases
                    ↓
WEEK 2
Existing ecosystem + platforms + workflows + friction
                    ↓
WEEK 3
User validation → MVP selection → PRD
```

The project is currently at the transition between Week 2 and Week 3.

---

# 3. What We Know

## 3.1 Kenya has an established climate-information ecosystem

Relevant climate, weather, environmental and humanitarian information
already exists through national, regional and global institutions and
platforms.

The ecosystem includes:

* national meteorological information;
* regional climate services;
* global climate datasets;
* Earth-observation data;
* humanitarian datasets;
* GIS and geospatial information;
* organizational/project datasets.

### Implication

The project should **not** begin with the assumption that Kenya lacks
climate data.

The more important question is whether users have difficulty turning
existing information into something useful for their work.

---

# 4. Multiple Providers and Platforms

Users may interact with several sources depending on their task.

Examples include:

* Kenya Meteorological Department;
* ICPAC;
* Copernicus;
* HDX;
* World Bank climate resources;
* Earth-observation platforms;
* research repositories;
* organizational datasets.

These systems serve different purposes.

### Implication

The project enters an existing ecosystem rather than an empty market.

The MVP therefore needs a clearly defined job that existing platforms
do not adequately address.

---

# 5. Existing User Workflows

The research suggests that climate-information workflows can contain
several stages:

```text
Information need
       ↓
Data discovery
       ↓
Dataset selection
       ↓
Data access
       ↓
Data preparation
       ↓
Data integration
       ↓
Analysis
       ↓
Interpretation
       ↓
Output
       ↓
Decision / action
```

Not every user performs every stage themselves.

Different organizations may divide these responsibilities between:

* programme staff;
* GIS specialists;
* information-management officers;
* researchers;
* developers;
* consultants;
* data analysts.

---

# 6. Current User Groups

The project currently considers three broad user groups.

## Primary

### NGOs / humanitarian / development organizations

Potential roles include:

* programme officers;
* GIS officers;
* information-management officers;
* monitoring and evaluation staff;
* climate/adaptation specialists;
* disaster-risk practitioners;
* data analysts.

These users are particularly relevant because climate information may
need to support operational or programme decisions.

---

## Secondary

### Researchers

Potential users include:

* climate researchers;
* environmental researchers;
* GIS researchers;
* hydrology/water researchers;
* agricultural researchers;
* disaster-risk researchers.

---

## Secondary

### Developers / GIS / data professionals

Potential users include people who:

* build applications;
* integrate APIs;
* process geospatial data;
* develop dashboards;
* create data pipelines.

---

# 7. What We Suspect

The following potential problems have emerged from the research.

They are **hypotheses rather than validated problems**.

---

## 7.1 Dataset discovery

Users may struggle to identify the most appropriate dataset among
multiple providers.

Possible causes:

* multiple sources;
* different terminology;
* different spatial resolutions;
* different temporal coverage;
* different methodologies;
* uncertainty about suitability.

### Status

**Hypothesis**

### Evidence needed

Determine how users actually find and select datasets.

---

# 8. Information Fragmentation

Relevant information may be distributed across multiple platforms.

A user may therefore have to:

```text
Platform A
   +
Platform B
   +
Platform C
   +
Internal data
   ↓
Complete analysis
```

### Potential consequence

Additional searching, downloading, processing and integration.

### Status

**Supported as an ecosystem characteristic; user impact not yet
validated.**

---

# 9. Data Access Friction

Different providers may use different mechanisms for accessing data,
including:

* web interfaces;
* downloads;
* APIs;
* registration;
* formal requests;
* machine-readable services.

### Potential problem

Users may have to learn different methods for different sources.

### Status

**Ecosystem characteristic; significance to users remains unvalidated.**

---

# 10. Manual Data Preparation

Users may need to perform operations such as:

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

### Potential consequence

Additional:

* time;
* technical effort;
* staff involvement;
* potential for errors.

### Status

**Hypothesis**

---

# 11. Climate + Contextual Data Integration

One of the most important hypotheses identified so far is that users
may need to combine climate information with other datasets.

For example:

```text
Climate data
      +
Administrative boundaries
      +
Population
      +
Programme locations
      +
Vulnerability
      ↓
Climate-risk analysis
      ↓
Operational information
```

### Why this matters

The user's actual question may not be:

> "What was the rainfall anomaly?"

It may instead be:

> "Which areas or programmes could be affected?"

### Status

**High-priority hypothesis**

This should receive significant attention during interviews.

---

# 12. Data → Decision Gap

Another potential gap exists between raw climate information and the
decision the user needs to support.

Possible chain:

```text
Data
 ↓
Processing
 ↓
Analysis
 ↓
Interpretation
 ↓
Decision
```

Existing platforms may be highly effective at supplying data but may
not necessarily address every downstream workflow.

### Status

**High-priority hypothesis**

### Research question

> "Once you have the climate information, what do you do with it?"

---

# 13. Technical Dependency

Some organizations may rely on specialist staff to obtain and process
climate information.

Possible workflow:

```text
Programme staff
      ↓
Information request
      ↓
GIS / data specialist
      ↓
Data discovery
      ↓
Processing
      ↓
Analysis
      ↓
Map / report
      ↓
Programme staff
```

### Potential problem

The person with the operational question may not be able to obtain the
answer independently.

### Important limitation

This is not necessarily inefficient.

Organizations may deliberately centralize technical expertise.

### Status

**Hypothesis**

---

# 14. Time to Usable Answer

A potentially important metric is:

```text
"I need this information"
            ↓
"I have a usable answer"
```

We currently do not know:

* how long this takes;
* which stage consumes most time;
* whether the time is considered excessive;
* whether the problem occurs frequently.

### Status

**Major evidence gap**

### Priority

**Very high**

---

# 15. Repeated Manual Workflows

Another potentially valuable problem is repeated work.

Example:

```text
Every week/month
       ↓
Find data
       ↓
Download
       ↓
Prepare
       ↓
Join
       ↓
Analyse
       ↓
Create output
```

If this occurs frequently, automation or workflow simplification may
provide meaningful value.

If it happens rarely, the opportunity may be significantly smaller.

### Status

**Major hypothesis**

### Priority

**Very high**

---

# 16. Dataset Trust and Selection

Users may need to determine whether a dataset is suitable based on:

* source;
* methodology;
* resolution;
* temporal coverage;
* update frequency;
* quality;
* licensing;
* intended use.

### Potential problem

Users may spend time evaluating which dataset to trust.

### Status

**Hypothesis**

---

# 17. Interoperability

Potential friction may arise from differences in:

* file formats;
* schemas;
* coordinate systems;
* geographic identifiers;
* spatial resolutions;
* temporal resolutions.

Example:

```text
GeoTIFF
CSV
NetCDF
JSON/API
Excel
```

### Status

**Hypothesis**

The actual burden on users needs to be established through interviews.

---

# 18. Developer/API Friction

Developers may encounter challenges involving:

* API documentation;
* authentication;
* rate limits;
* endpoint structure;
* data formats;
* historical data;
* licensing;
* reliability;
* update mechanisms.

### Status

**Hypothesis**

This is relevant to the secondary developer user group but should not
displace the primary user research.

---

# 19. Consolidated Friction Matrix

| #  | Potential friction                                  | Main users               | Workflow stage | Current evidence    | Status                   | Research priority |
| -- | --------------------------------------------------- | ------------------------ | -------------- | ------------------- | ------------------------ | ----------------- |
| 1  | Difficulty discovering appropriate datasets         | Researchers / NGOs       | Discovery      | Multiple providers  | Hypothesis               | High              |
| 2  | Information distributed across platforms            | Researchers / NGOs       | Discovery      | Ecosystem research  | Supported characteristic | High              |
| 3  | Different access mechanisms                         | All                      | Access         | Platform research   | Supported characteristic | Medium            |
| 4  | Manual data preparation                             | Researchers / NGOs       | Processing     | Workflow analysis   | Hypothesis               | High              |
| 5  | Climate + contextual data integration               | NGOs / humanitarian      | Integration    | Workflow analysis   | High-priority hypothesis | **Very High**     |
| 6  | Data does not directly answer operational questions | NGOs / development       | Interpretation | Workflow hypothesis | High-priority hypothesis | **Very High**     |
| 7  | Dependence on technical specialists                 | NGOs                     | Processing     | Workflow hypothesis | Hypothesis               | High              |
| 8  | Long time from question to answer                   | All                      | End-to-end     | No primary evidence | Unknown                  | **Very High**     |
| 9  | Repeated manual workflows                           | NGOs / researchers       | Processing     | No primary evidence | Unknown                  | **Very High**     |
| 10 | Difficulty evaluating datasets                      | Researchers / NGOs       | Discovery      | Platform complexity | Hypothesis               | Medium            |
| 11 | Interoperability problems                           | Researchers / developers | Integration    | Technical analysis  | Hypothesis               | Medium            |
| 12 | API/integration difficulties                        | Developers               | Access         | Technical analysis  | Hypothesis               | Medium            |

---

# 20. Preliminary Opportunity Gaps

These are **research opportunities**, not confirmed product features.

## Opportunity 1 — Better discovery

Potential opportunity:

> Make relevant climate information easier to discover and understand.

### Challenge

Existing catalogues already provide discovery capabilities.

The research must identify what remains unresolved.

---

## Opportunity 2 — Data integration

Potential opportunity:

> Reduce the effort required to combine climate information with
> contextual or programme data.

### Research question

Do users actually perform this integration frequently enough for it to
matter?

---

## Opportunity 3 — Reusable workflows

Potential opportunity:

> Reduce repeated manual processing of commonly used datasets.

### Research question

Which workflows are repeated and how much effort do they consume?

---

## Opportunity 4 — Decision-oriented information

Potential opportunity:

> Help users move from climate indicators to information relevant to a
> specific operational or programme question.

### Research question

Is the problem actually data access, interpretation, or something else?

---

## Opportunity 5 — Kenya-focused contextualization

Potential opportunity:

> Present climate information in a way that reflects Kenyan
> administrative, programme and development contexts.

### Research question

What specifically is missing from existing global and regional
platforms?

---

# 21. What We Should Not Assume

The following assumptions remain unproven:

* Users need another climate-data repository.
* Users cannot find climate data.
* Existing platforms are inadequate.
* NGOs want an AI climate assistant.
* Users want a single dashboard.
* Users want everything in one platform.
* Users would pay for the service.
* The main problem is technical.
* The main problem is data availability.
* The solution must be a website.
* The initial product should cover all of Africa.

These should not become product requirements without supporting
evidence.

---

# 22. What Could Challenge the Project

The research may discover that:

### Scenario A — Existing systems are sufficient

Users already have effective internal workflows.

**Implication:** The proposed product may not address a sufficiently
important problem.

---

### Scenario B — The problem is primarily skills/training

Users may have access to appropriate data but lack the skills to use it.

**Implication:** Training, documentation or services could be more
appropriate than software.

---

### Scenario C — The problem is data licensing/access

Users may know exactly what they need but cannot access the required
datasets.

**Implication:** Data partnerships/licensing may become more important
than platform development.

---

### Scenario D — Users need specialist analysis

The workflows may be too specialized for a general-purpose platform.

**Implication:** A focused service or specialized tool may be more
appropriate.

---

### Scenario E — Contextual data is the actual bottleneck

Users may already have climate data but lack the contextual datasets
needed to interpret it.

**Implication:** Data integration could become a central research
direction.

---

### Scenario F — The problem is organizational

The main barrier could involve:

* decision processes;
* responsibilities;
* budgets;
* communication;
* staffing.

**Implication:** Technology alone may not solve the problem.

---

# 23. Week 3 Questions

Before selecting the MVP, the following questions need evidence.

## User

1. Who experiences the problem most frequently?
2. Who is responsible for solving it?
3. Who ultimately uses the information?

## Workflow

4. What does the current workflow look like?
5. Which steps are manual?
6. Which steps are repeated?
7. Which tools are used?

## Frequency

8. How often does the problem occur?
9. Is it recurring or occasional?

## Effort

10. How much time does it consume?
11. How many people are involved?
12. What technical skills are required?

## Consequences

13. What happens when the workflow fails or takes too long?
14. Does it delay reporting or decisions?
15. Does it create additional costs?

## Existing alternatives

16. Which platforms are already used?
17. What internal workarounds exist?
18. Why have users not already solved the problem?

## Value

19. What would users actually want improved?
20. What would that improvement save?
21. Would it change their current workflow?

## Product scope

22. Does this problem require a new product?
23. Could an existing platform, API or workflow solve it?
24. What is the smallest useful solution?

---

# 24. MVP Selection Criteria

At the end of Week 3, a candidate MVP problem should ideally satisfy
most of the following:

| Criterion           | Question                                                          |
| ------------------- | ----------------------------------------------------------------- |
| Real                | Have actual users experienced it?                                 |
| Recurring           | Does it happen repeatedly or matter significantly when it occurs? |
| Specific            | Can the problem be described precisely?                           |
| Important           | Does it have meaningful consequences?                             |
| Existing workaround | Are users already spending effort solving it?                     |
| Reachable           | Can we access the users and data required?                        |
| Feasible            | Can we build a small solution?                                    |
| Differentiated      | Does it address a gap not adequately handled by existing systems? |
| Testable            | Can we measure whether our solution improves the workflow?        |

The MVP should be selected **after** the evidence is collected.

---

# 25. Current Project Hypothesis

The current research can be represented as:

```text
AVAILABLE CLIMATE INFORMATION
             ↓
     Multiple providers
             ↓
      Multiple platforms
             ↓
       Multiple formats
             ↓
             ?
             ↓
       USER WORKFLOW
             ↓
   Processing / integration
             ↓
          Context
             ↓
          Analysis
             ↓
          Decision
```

The central research question is:

> **Where does meaningful friction actually occur between available
> climate information and the user's desired outcome?**

---

# 26. Provisional Problem Statement

For the transition into Week 3, use the following as the working
problem statement:

> **Climate and weather information relevant to Kenya is available
> through multiple national, regional and global sources. However,
> users may still face difficulties discovering appropriate datasets,
> accessing and preparing them, combining them with contextual
> information, and translating the resulting analysis into useful
> research, humanitarian, development or operational outputs.**

This statement remains provisional.

It should be revised after primary user research.

---

# 27. Evidence Required Before MVP Selection

The following evidence should be collected during Week 3:

* [ ] At least several relevant user interviews
* [ ] Concrete examples of recent workflows
* [ ] Recurring problems identified
* [ ] Frequency of problems established
* [ ] Approximate time/effort established
* [ ] Existing workarounds documented
* [ ] Consequences documented
* [ ] Existing platforms/tools documented from user experience
* [ ] User priorities compared
* [ ] Contradictory evidence documented
* [ ] Candidate MVP problem identified
* [ ] MVP scope defined
* [ ] PRD drafted

---

# 28. What Day 14 Has Established

## We know

* Kenya has substantial climate-information infrastructure.
* Relevant national, regional and global data sources exist.
* Multiple platforms already serve parts of the ecosystem.
* Users have different technical roles and workflows.
* Potential friction exists across discovery, access, processing,
  integration and interpretation.

## We suspect

* Data fragmentation may create workflow friction.
* Data preparation may involve repetitive manual work.
* Climate information may need to be combined with contextual data.
* NGOs and humanitarian organizations may need more
  decision-oriented information.
* Some users may depend heavily on GIS/data specialists.

## We do not yet know

* Which problem is most important.
* Which users experience it most strongly.
* How frequently it occurs.
* How much time it consumes.
* What the existing workaround costs.
* Whether users would change their workflow.
* Whether a new product is actually required.

---

# 29. Transition to Week 3

The project should now move from:

> **"What problems might exist?"**

to:

> **"Which problems do real users actually experience?"**

Then:

```text
User evidence
      ↓
Validated/challenged problems
      ↓
Problem prioritization
      ↓
MVP problem
      ↓
MVP user
      ↓
Jobs-to-be-done
      ↓
MVP scope
      ↓
Product Requirements Document
```

The original Week 3 objective remains unchanged:

> **Select the MVP and write the Product Requirements Document (PRD).**

---

# 30. Day 14 Status

| Deliverable                                   | Status     |
| --------------------------------------------- | ---------- |
| Consolidate ecosystem findings                | ✅ Complete |
| Consolidate workflow findings                 | ✅ Complete |
| Consolidate friction findings                 | ✅ Complete |
| Separate evidence from hypotheses             | ✅ Complete |
| Identify opportunity gaps                     | ✅ Complete |
| Identify assumptions that could be challenged | ✅ Complete |
| Define Week 3 questions                       | ✅ Complete |
| Select MVP                                    | ⏳ Week 3   |
| Write PRD                                     | ⏳ Week 3   |

**Day 14 is complete.**

The next stage is **Week 3: user validation → MVP selection → PRD**.

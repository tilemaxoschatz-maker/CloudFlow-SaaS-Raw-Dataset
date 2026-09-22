# CloudFlow SaaS Revenue, Retention, Product & Growth Analytics

**End-to-end B2B SaaS analytics portfolio project built natively in Google Sheets**

This project transforms eight connected source datasets into a controlled analytical workbook covering **recurring revenue, subscription retention, customer growth, product adoption, support performance, invoice collection, and marketing efficiency**.

The final deliverable combines data documentation, quality controls, clean layers, analytical models, five detailed analysis sheets, an executive dashboard, an executive insight brief, and a PowerPoint presentation.

> **Best viewing experience:** open the native Google Sheets workbook below. The Excel export is useful as a local copy, but some chart positions, formatting, merged cells, and Google Sheets-specific formulas may display differently in Microsoft Excel.

## Live Project

**[▶ View the full native Google Sheets workbook](https://docs.google.com/spreadsheets/d/1aB6EJyum1TMhO1PrAaIwPElv_bpxdSFA2bQxTE7J2KI/edit)**

### Downloads

- **[Download the Excel export](https://docs.google.com/spreadsheets/d/1aB6EJyum1TMhO1PrAaIwPElv_bpxdSFA2bQxTE7J2KI/export?format=xlsx)**
- **[Download the executive PowerPoint presentation](./CloudFlow_SaaS_Analytics_Project_Final_v2.pptx)**

---
## Dashboard Preview

<p align="center">
  <img src="https://github.com/tilemaxoschatz-maker/CloudFlow-SaaS-Raw-Dataset/blob/main/dashboard_review/Screenshot%202026-09-22%20153752.png">
</p>

<p align="center">
  <img src="https://github.com/tilemaxoschatz-maker/CloudFlow-SaaS-Raw-Dataset/blob/main/dashboard_review/Screenshot%202026-09-22%20153830.png">
</p>

---
## Project Overview

| Item | Description |
|---|---|
| **Company** | CloudFlow, a synthetic B2B SaaS company offering workflow-automation software |
| **Business objective** | Evaluate recurring revenue, retention, customer behavior, product adoption, service quality, cash collection, and acquisition efficiency |
| **Analysis period** | January 2023 to December 2025 |
| **Source structure** | Eight connected raw datasets covering customers, plans, subscriptions, events, invoices, usage, support, and marketing |
| **Primary tool** | Google Sheets |
| **Supporting techniques** | Data auditing, cleaning, lookup-based modeling, reconciliation controls, calculated KPIs, charts, and executive reporting |
| **Main outputs** | 34-tab analytical workbook, executive dashboard, executive insight brief, and PowerPoint presentation |
| **Dataset type** | Fully synthetic portfolio dataset |

---

## Business Objective

The project addresses a management-level question:

> **How is CloudFlow performing across growth, retention, product adoption, customer service, cash collection, and acquisition efficiency, and which issues should leadership address first?**

The analysis goes beyond reporting total revenue. It evaluates whether growth is sustainable, whether existing customers are expanding or contracting, whether customers are adopting the product, whether support operations can serve the growing customer base, and whether marketing investment is producing efficient acquisition.

---

## Business Questions

1. How are monthly recurring revenue and annual recurring revenue changing?
2. How quickly is the active subscription base growing?
3. What is driving new MRR, expansion, contraction, and churned MRR?
4. How are gross logo churn, gross revenue churn, and net revenue retention changing?
5. Which subscription cohorts and customer segments retain best?
6. How does product adoption differ by plan, region, lifecycle stage, and customer segment?
7. How effectively are licensed seats being used?
8. How are support volume, SLA attainment, response time, resolution time, and CSAT changing?
9. How effectively does CloudFlow collect invoiced revenue?
10. Which acquisition channels report the strongest customer-acquisition efficiency?
11. How reliable is the available CRM attribution for marketing decisions?
12. Which findings represent real business signals, and which require source validation?

---

## Analytical Workflow

```text
RAW SOURCE TABLES
        ↓
DATA DICTIONARY & AUDIT
        ↓
CLEAN DATA LAYERS
        ↓
RECONCILIATION CONTROLS
        ↓
ANALYTICAL MODEL TABLES
        ↓
FIVE ANALYSIS SHEETS
        ↓
EXECUTIVE DASHBOARD
        ↓
EXECUTIVE INSIGHT
        ↓
POWERPOINT PRESENTATION
```

The workbook follows a controlled end-to-end analytics process:

1. **Project definition** - documents the company, reporting period, business questions, and expected deliverables.
2. **Raw-data preservation** - keeps the original exports unchanged for traceability.
3. **Data dictionary** - records field definitions and expected business meaning.
4. **Data audit** - checks row counts, keys, missing values, date rules, chronology, and relationships.
5. **Data-quality assessment** - records nine material issues, their business impact, and the selected treatment.
6. **Clean-layer development** - standardizes valid fields and removes only confirmed exact duplicates.
7. **Reconciliation controls** - confirms row preservation, measure preservation, deduplication, and foreign-key integrity.
8. **Analytical modeling** - enriches transactional tables with customer, plan, lifecycle, time, and KPI-ready fields.
9. **Business analysis** - evaluates revenue, retention, adoption, support operations, and marketing performance.
10. **Dashboard development** - presents the most important KPIs and charts in a management-ready layout.
11. **Executive interpretation** - converts the analysis into business conclusions, risks, and recommended actions.
12. **Executive presentation** - communicates the project and its major findings in a concise nine-slide PowerPoint deck.

---

## Source Data

| Source table | Business content | Raw records |
|---|---|---:|
| `RAW_CUSTOMERS` | Customer profile, geography, segment, industry, acquisition details, and signup date | 1,600 |
| `RAW_PLANS` | Subscription-plan attributes and commercial terms | 8 |
| `RAW_SUBSCRIPTIONS` | Subscription ownership, plan, status, seats, and lifecycle dates | 2,600 |
| `RAW_SUBSCRIPTION_EVENTS` | Activations, upgrades, downgrades, cancellations, seats, and MRR movements | 6,349 |
| `RAW_INVOICES` | Billing, discounts, refunds, payment status, dates, and collected cash | 16,012 |
| `RAW_USAGE_MONTHLY` | Monthly users, seats, product activity, storage, API calls, projects, automations, and logins | 26,000 |
| `RAW_SUPPORT` | Ticket priority, timestamps, SLA targets, CSAT, reopen, and escalation fields | 3,508 |
| `RAW_MARKETING_SPEND` | Monthly campaign spend, impressions, clicks, leads, trials, and reported customers | 288 |

---

## Workbook Structure

### Documentation and Controls

| Worksheet | Purpose |
|---|---|
| `PROJECT_BRIEF` | Company context, analysis period, project objective, and core business questions |
| `Data Dictionary` | Field definitions and source documentation |
| `DATA_AUDIT` | Row counts, uniqueness checks, date checks, rule checks, and relationship validation |
| `DATA_QUALITY` | Material data-quality findings, severity, impact, treatment, and status |
| `RECONCILIATION_CONTROL` | Raw-to-clean reconciliation, duplicate controls, measure preservation, and modeling restrictions |

### Raw Source Tables

| Worksheet | Purpose |
|---|---|
| `RAW_CUSTOMERS` | Original customer records |
| `RAW_PLANS` | Original subscription-plan master |
| `RAW_SUBSCRIPTIONS` | Original subscription records |
| `RAW_SUBSCRIPTION_EVENTS` | Original subscription lifecycle events |
| `RAW_INVOICES` | Original invoice and payment records |
| `RAW_USAGE_MONTHLY` | Original monthly product-usage observations |
| `RAW_SUPPORT` | Original support-ticket records |
| `RAW_MARKETING_SPEND` | Original campaign and acquisition data |

### Clean Data Layers

| Worksheet | Purpose |
|---|---|
| `CLEAN_CUSTOMER` | Standardized customer records with date-quality controls |
| `CLEAN_PLANS` | Preserved eight-plan reference table |
| `CLEAN_SUBSCRIPTIONS` | Standardized subscription records with lifecycle fields retained |
| `CLEAN_SUBSCRIPTION_EVENTS` | Event table after removing 14 confirmed exact duplicates |
| `CLEAN_INVOICES` | Invoice table after removing 12 confirmed exact duplicates and flagging invalid date intervals |
| `CLEAN_USAGE_MONTHLY` | Preserved usage observations with normalized valid dates and grain-quality flags |
| `CLEAN_SUPPORT` | Support table after removing eight exact duplicates and flagging invalid timing records |
| `CLEAN_MARKETING_SPEND` | Standardized marketing data covering 36 months and all expected month-channel combinations |

### Analytical Models

| Worksheet | Purpose |
|---|---|
| `MODEL_SUBSCRIPTIONS` | Subscription model enriched with customer and plan attributes |
| `MODEL_SUBSCRIPTION_EVENTS` | Lifecycle and MRR-movement model for growth and retention analysis |
| `MODEL_INVOICES` | Billing, collection, payment-status, and invoice-timing model |
| `MODEL_USAGE_MONTHLY` | Usage model enriched with subscription, customer, plan, lifecycle, and quality fields |
| `MODEL_SUPPORT` | Support model enriched with customer context and valid KPI-eligibility flags |
| `MODEL_MARKETING` | Marketing-performance model with funnel and efficiency calculations |

### Analysis and Executive Outputs

| Worksheet | Purpose |
|---|---|
| `ANALYSIS_KPI_MONTHLY` | Monthly growth, recurring revenue, churn, retention, billing, and collection KPIs |
| `ANALYSIS_REVENUE_RETENTION` | Revenue movements, logo churn, revenue churn, NRR, and subscription-cohort retention |
| `ANALYSIS_USAGE_ADOPTION` | Monthly usage trends and adoption comparisons by plan, region, lifecycle stage, and segment |
| `ANALYSIS_SUPPORT` | Monthly support performance and comparisons by priority, issue type, plan, region, and segment |
| `ANALYSIS_MARKETING` | Monthly and annual acquisition performance by channel, campaign, and region |
| `DASHBOARD` | Executive KPI cards and the most important analytical charts |
| `EXECUTIVE_INSIGHT` | Executive summary, prioritized findings, recommended actions, KPI comparisons, and caveats |

---

## Data-Quality Findings and Treatment

The audit identified **nine material findings: four High, four Medium, and one Low**.

| Area | Finding | Treatment |
|---|---|---|
| Customer dates | 1,600 signup dates contained hidden time components | Converted valid values to date-only fields in the clean layer |
| Subscription events | 14 excess duplicate event records | Removed only confirmed exact duplicates |
| Invoice keys | 12 excess duplicate invoice records | Removed only confirmed exact duplicates and preserved source references |
| Invoice dates | 310 date-rule violations | Retained source values, added flags, and excluded invalid intervals from timing KPIs |
| Monthly usage grain | 10,558 excess subscription-month observations with conflicting measures | Preserved all records and labelled aggregated usage measures as proxy estimates |
| Usage dates | 26 usage-date rule violations | Normalized valid month fields and flagged invalid sequences |
| Support ticket keys | Eight excess duplicate ticket records | Removed only confirmed exact duplicates |
| Support chronology | Eight timestamp-rule violations | Preserved records for volume analysis and excluded invalid timing intervals from duration KPIs |
| Support measures | Eight range or consistency violations | Added eligibility flags and excluded invalid measures from affected KPI denominators |

### Reconciliation Result

| Control outcome | Result |
|---|---:|
| **Controls passed** | **10** |
| **Controls for review** | **2** |
| **Critical control failures** | **0** |
| **Data-grain or KPI limitations** | **2** |
| **Modeling status** | **Ready with restrictions** |

The reconciliation confirms that the raw-to-clean pipelines preserve required records, financial measures, and key relationships. The two remaining restrictions concern unresolved monthly usage grain and four support tickets with invalid resolution chronology.

---

## Engineered Features and Calculated Metrics

The model layers add business-ready fields including:

- Customer segment, region, industry, acquisition channel, and campaign
- Plan name, tier, billing frequency, included seats, and commercial limits
- Subscription start, trial-end, cancellation, renewal, and lifecycle fields
- Year, quarter, month, and year-month reporting dimensions
- New, expansion, contraction, and churned MRR
- Beginning and ending active subscriptions
- Beginning and ending MRR
- Monthly and annual recurring revenue
- Gross logo churn rate
- Gross revenue churn rate
- Net revenue retention
- Invoice cohort collection rate
- Collection-issue indicators
- First-response and resolution duration validity flags
- SLA-eligible and SLA-met indicators
- CSAT-response eligibility
- Seat-utilization estimates
- Product-adoption estimates
- Marketing funnel conversion rates
- Customer acquisition cost
- CRM attribution coverage

These variables support a single analytical flow from source records to executive decisions while keeping source limitations visible.

---

## December 2025 Executive Snapshot

| KPI | Result | Comparison or context |
|---|---:|---|
| **Ending MRR** | **$491,471** | Up 135.6% from December 2024 |
| **Ending ARR** | **$5.90M** | Based on December ending MRR |
| **Active subscriptions** | **2,007** | Up 114.4% from December 2024 |
| **Net revenue retention** | **96.5%** | Down 4.1 percentage points year over year |
| **Gross logo churn** | **4.6%** | 96 cancellations against 2,103 beginning subscriptions |
| **Invoice-cohort collection rate** | **93.2%** | 57 collection-issue invoices |
| **Estimated seat utilization** | **62.3%** | Proxy usage measure |
| **Estimated feature-adoption score** | **54.8** | Proxy usage measure |
| **First-response SLA met** | **40.4%** | 151 of 374 eligible tickets met SLA |
| **Average first-response time** | **14.2 hours** | Valid timing records only |
| **Average resolution time** | **53.3 hours** | Valid chronology records only |
| **Average CSAT** | **3.93 / 5** | 235 December responses |

> **Usage limitation:** seat-utilization and feature-adoption values are directional proxy estimates. The source contains conflicting observations at the subscription-month grain, so the analysis averages those observations until source precedence is confirmed.

---

# Key Business Insights

## 1. CloudFlow achieved substantial scale, but growth reversed at year-end

December 2025 MRR reached approximately **$491.5K**, up **135.6% year over year**, while active subscriptions reached **2,007**, up **114.4%**.

However, MRR peaked at approximately **$518.5K in October 2025** and declined **5.2%** by December. Active subscriptions declined **9.6%** over the same period.

**Business implication:** historical growth remains strong, but leadership should focus on restoring positive net subscription additions and preventing further contraction.

---

## 2. Retention weakened below the expansion threshold

Net revenue retention declined from **100.6% in December 2024** to **96.5% in December 2025**.

December churned MRR reached approximately **$17.7K**, while no new or expansion MRR was recorded during the month.

**Business implication:** existing-customer contraction and churn now exceed expansion, placing more pressure on acquisition and customer-success performance.

---

## 3. The model records no new activations in November or December

CloudFlow recorded **135 new activations in October 2025**, followed by **zero in November and December**. Cancellations reached **116 in November** and **96 in December**.

**Business implication:** this could represent a major acquisition interruption or a source-timing issue. Leadership should validate the underlying event data before treating it as a confirmed pipeline shutdown.

---

## 4. SMB product adoption trails Enterprise customers

Proxy usage estimates show an Enterprise feature-adoption score of **68.2**, compared with **48.9 for SMB**, a difference of **19.3 points**.

Estimated seat utilization is **68.7% for Enterprise** and **53.3% for SMB**.

**Business implication:** SMB customers appear to realize less product value. More structured activation and onboarding could improve usage depth and reduce future churn risk.

---

## 5. Support service reliability remains weak

December first-response SLA attainment was **40.4%**. Average first-response time was **14.2 hours**, average resolution time was **53.3 hours**, and CSAT was **3.93 out of 5**.

SLA performance remains weak across customer segments and ticket priorities rather than being limited to one category.

**Business implication:** CloudFlow needs operational improvements in staffing, queue ownership, prioritization, and backlog management.

---

## 6. Marketing acquisition became less efficient in 2025

Compared with 2024:

- Marketing spend increased **3.3%** to approximately **$1.88M**.
- Reported acquired customers declined **11.7%** to **4,079**.
- Blended customer acquisition cost increased **17.0%** to approximately **$461**.

Paid Social reported the lowest channel CAC at approximately **$260**, while Partner and Events reported approximately **$539** and **$512**.

**Business implication:** channel efficiency differs materially, but major budget shifts should wait until attribution quality improves.

---

## 7. Marketing attribution is not reliable enough for revenue-return decisions

CRM attribution covered only **0.64% of reported 2025 acquired customers** and **0% in December 2025**.

**Business implication:** channel CAC can support directional testing, but it should not be interpreted as fully attributed revenue return or used alone for large budget reallocations.

---

## 8. Collection performance is strong but still requires targeted follow-up

The December invoice-cohort collection rate was **93.2%**, with **57 invoices** identified as collection issues.

**Business implication:** broad collection performance is healthy, but unresolved invoices should be segmented by payment status, customer value, age, and failure reason.

---

# Strategic Recommendations

### 1. Restore acquisition and retention momentum

Validate the zero-activation result for November and December. Establish a weekly operating review of new activations, cancellations, new MRR, expansion MRR, churned MRR, and NRR.

### 2. Repair attribution before reallocating marketing spend

Implement consistent campaign-level CRM tracking. Use Paid Social as an efficiency benchmark, but require verified conversion evidence before making major channel-budget changes.

### 3. Launch an SMB adoption program

Adapt the strongest Enterprise onboarding practices for SMB customers. Monitor activation milestones, seat utilization, feature adoption, and repeat workflow creation.

### 4. Stabilize support SLA performance

Review demand, staffing, and backlog by priority. Assign clear queue ownership and monitor response-time and resolution-time delays every week.

### 5. Protect invoice collection

Create a targeted review of collection-issue invoices by account value, payment status, aging, and customer segment.

---

## Dashboard Design

The executive dashboard is designed for fast management review.

```text
EXECUTIVE HEADER
      ↓
SIX HEADLINE KPIs
      ↓
REVENUE & SUBSCRIPTION TRENDS
      ↓
RETENTION & CHURN
      ↓
PRODUCT ADOPTION
      ↓
SUPPORT PERFORMANCE
      ↓
MARKETING EFFICIENCY
```

The six headline KPIs are:

- Ending MRR
- Active subscriptions
- Net revenue retention
- Estimated seat utilization
- Support SLA met
- Marketing CAC

The dashboard intentionally presents only the most important charts. Detailed calculations and segment comparisons remain in the five analysis sheets.

---

## Executive Presentation

The PowerPoint presentation converts the workbook into a concise nine-slide management narrative. It is intended for portfolio reviewers and business stakeholders who want to understand the project without navigating every worksheet.

The presentation covers:

1. Project objective and analytical architecture
2. Data-quality findings and reconciliation controls
3. December 2025 executive snapshot
4. MRR growth and the year-end reversal
5. Product-adoption differences by customer segment
6. Support SLA performance
7. Marketing efficiency by acquisition channel
8. Management recommendations and success measures

### Presentation Preview

<p align="center">
  <img src="https://github.com/tilemaxoschatz-maker/CloudFlow-SaaS-Raw-Dataset/blob/main/presentation_review/Screenshot%202026-09-22%20160453.png">
</p>

<p align="center">
  <img src="https://github.com/tilemaxoschatz-maker/CloudFlow-SaaS-Raw-Dataset/blob/main/presentation_review/Screenshot%202026-09-22%20160524.png">
</p>

**[Download the full executive PowerPoint presentation](./CloudFlow_SaaS_Analytics_Project_Final_v2.pptx)**

---

## Repository Structure

```text
CloudFlow-SaaS-Analytics/
├── README.md
└── CloudFlow_SaaS_Analytics_Project_Final_v2.pptx
```

The live Google Sheets workbook remains the primary analytical artifact and is linked at the top of this README.

---

## How to Use the Project

1. Open the native Google Sheets workbook for the intended layout and formatting.
2. Read `PROJECT_BRIEF` to understand the business context and project scope.
3. Use `Data Dictionary` to review the field definitions.
4. Review `DATA_AUDIT` and `DATA_QUALITY` to understand the source issues.
5. Review the `CLEAN_*` sheets to see the cleaning decisions and quality flags.
6. Use `RECONCILIATION_CONTROL` to confirm row, measure, and relationship integrity.
7. Review the `MODEL_*` sheets to understand how the analytical tables were enriched.
8. Use `ANALYSIS_KPI_MONTHLY` for the complete monthly KPI framework.
9. Review the four specialized analysis sheets for retention, adoption, support, and marketing detail.
10. Open `DASHBOARD` for the executive visual summary.
11. Read `EXECUTIVE_INSIGHT` for the prioritized findings, actions, comparisons, and caveats.
12. Download the PowerPoint presentation for the final management narrative.
13. Use the Excel export only when a local copy is required. Native Google Sheets remains the preferred viewing format.

---

## Skills Demonstrated

### Data Preparation and Governance

- Multi-table data auditing
- Source-data preservation
- Data-dictionary development
- Duplicate-key assessment
- Date and chronology validation
- Missing-value and rule validation
- Data-quality issue documentation
- Reconciliation-control design
- Record-level traceability

### Data Cleaning

- Exact-duplicate removal
- Date normalization
- Controlled handling of invalid intervals
- KPI-eligibility flags
- Grain validation
- Preserving unresolved source observations
- Documenting cleaning decisions and restrictions

### Data Modeling

- Multi-table integration
- Customer and plan enrichment
- Subscription lifecycle modeling
- Event-based MRR modeling
- Invoice and collection modeling
- Usage and adoption modeling
- Support-operational modeling
- Marketing-funnel modeling
- Foreign-key and ownership validation

### Spreadsheet Analytics

- Google Sheets
- Microsoft Excel interoperability
- `XLOOKUP`
- `SUMIFS`
- `COUNTIFS`
- `COUNTA`
- `FILTER`
- `QUERY`
- `UNIQUE`
- `COUNTUNIQUE`
- `AVERAGEIFS`
- `IF`
- `IFERROR`
- Date and month functions
- Dynamic KPI calculations

### SaaS and Revenue Analytics

- Monthly recurring revenue
- Annual recurring revenue
- New, expansion, contraction, and churned MRR
- Gross logo churn
- Gross revenue churn
- Net revenue retention
- Active-subscription tracking
- Subscription-cohort retention
- Invoice collection

### Product and Customer Analytics

- Product-adoption scoring
- Seat-utilization analysis
- Customer-segment comparison
- Plan analysis
- Regional analysis
- Lifecycle-stage analysis
- Usage-quality assessment

### Operational Analytics

- Ticket-volume analysis
- SLA-eligibility logic
- First-response performance
- Resolution-time analysis
- CSAT reporting
- Support-quality controls
- Priority and customer-segment comparisons

### Marketing Analytics

- Spend and acquisition analysis
- Funnel-conversion rates
- Customer acquisition cost
- Channel and campaign comparison
- Regional marketing performance
- CRM attribution coverage
- Data-quality-aware budget recommendations

### Data Visualization and Communication

- Executive dashboard design
- KPI cards
- Time-series charts
- Segment comparisons
- Channel-efficiency charts
- Executive insight writing
- Management recommendations
- PowerPoint storytelling
- Portfolio case-study development

---

## Tools

- **Google Sheets**
- **Microsoft Excel**
- **Microsoft PowerPoint**
- Spreadsheet formulas
- Lookup-based modeling
- Data reconciliation
- Feature engineering
- Data visualization
- SaaS KPI analysis
- Business analytics

---

## Important Analytical Caveats

1. **Synthetic dataset:** the project does not describe a real company or real customers.
2. **Usage grain:** conflicting subscription-month usage observations prevent authoritative usage aggregation. Reported usage KPIs are proxy estimates.
3. **Support timing:** invalid chronology records are excluded from timing and SLA calculations but retained for ticket-volume analysis.
4. **Activation completeness:** zero activations in November and December 2025 require source validation before being treated as a confirmed business event.
5. **Marketing attribution:** low CRM coverage limits revenue-return conclusions and large channel-budget decisions.
6. **Causality:** plan, segment, region, and channel differences are descriptive and do not prove that the category caused the observed result.

---

## Disclaimer

This project is intended for **portfolio and educational purposes**. CloudFlow and all underlying records are synthetic. The results demonstrate an end-to-end SaaS analytics workflow and should not be interpreted as the performance of a real company.

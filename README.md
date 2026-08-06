# Welfare Delivery Gap Analysis — PM-KISAN, MGNREGA & PMAY-G

## Overview
This project analyses the gap between welfare entitlement and actual delivery 
across three major Indian government schemes — PM-KISAN, MGNREGA, and PMAY-G. 
Using official government MIS data, CAG audit reports, and PFMS payment records, 
it constructs a state-level Delivery Efficiency Score (DES) to identify where 
and why welfare transfers fail to reach intended beneficiaries.

## Research Question
Which Indian states show the largest gap between eligible beneficiaries and 
actual delivery — and what structural factors predict this gap?

## Schemes Analysed
- **PM-KISAN** — Direct income support to farmer households (₹6,000/year via DBT)
- **MGNREGA** — Guaranteed rural employment (100 days/year wage entitlement)
- **PMAY-G** — Rural housing construction subsidy (₹1.2–1.4 lakh in tranches)

## Three Core Problems Measured
| Problem | Definition |
|---|---|
| Exclusion Error | Eligible beneficiaries not registered or receiving benefits |
| Inclusion Error | Ineligible or ghost beneficiaries receiving transfers |
| Payment Failure | Registered beneficiaries approved but payment not received |

## Data Sources
| Dataset | Source | Use in Project |
|---|---|---|
| MGNREGA MIS (Job Cards, Person-Days, Wage Payments) | nrega.nic.in | Primary MGNREGA delivery data |
| PM-KISAN MIS (Beneficiary and Payment Status) | pmkisan.gov.in | Primary PM-KISAN delivery data |
| PMAY-G AwaasSoft (Targets vs Achievement, Instalments) | pmayg.nic.in | Primary PMAY-G delivery data |
| SECC 2011 | secc.gov.in / MoRD | Eligible universe benchmark |
| PFMS Payment Records | pfms.nic.in | Payment pipeline failure analysis |
| CAG Audit Reports | cag.gov.in | Leakage and audit evidence |
| DBT Bharat Portal | dbtbharat.gov.in | National transfer context |

## Tools Used
- **Python** — Data cleaning, merging, index construction, regression analysis
- **SQL** — Structured querying and state-level aggregations
- **Excel** — Initial exploration and scheme comparison matrix
- **Power BI / Tableau** — Interactive dashboard and choropleth maps
- **Policy Writing** — 1200-word policy brief with recommendations

## Repository Structure
welfare-delivery-gap-india/
│
├── data/
│ ├── raw/ # Original downloaded government datasets
│ └── cleaned/ # Processed and merged datasets
│
├── notebooks/ # Python notebooks for cleaning, analysis, index
│
├── outputs/
│ ├── charts/ # Static visualisation exports
│ └── dashboard/ # Power BI / Tableau dashboard files
│
├── brief/ # Final policy brief PDF
│
└── README.md
## Key Output — Delivery Efficiency Score (DES)
A composite index built from three normalised variables per state:
1. Coverage gap rate (exclusion error)
2. Inclusion error rate (ghost/ineligible beneficiaries)
3. Payment failure rate (DBT pipeline failures)

States are ranked on DES across all three schemes to identify 
systemic delivery bottlenecks.

## Status
🟡 In Progress — Week 2 started (Data Collection)

## Author
Geetika | B.Tech ICT | Public Policy & Data Analytics
[LinkedIn](https://www.linkedin.com/in/geetika-chandrashekhar/) | [GitHub](https://github.com/geetify1601)

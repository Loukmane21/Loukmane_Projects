# Bouygues Telecom — Data Engineering & Predictive Analytics

**Professional case study** · Python · VBA · SQL · Docker · Streamlit · Predictive modelling

> This case study describes my contributions at a high level. No source code, internal datasets, confidential metrics, or proprietary architecture details are shared.

## Overview

My work covered two complementary topics: modernising an existing data-processing workflow and making quantitative sales analysis more accessible to business teams.

## 1. Modernising a VBA-based data-processing workflow

### Starting point

I took over an existing stack built around VBA macros. Before changing it, I needed to understand how the full process worked in production: where data came from, how it moved through the different processing stages, how transformations were applied, and how downstream teams and applications used the resulting data.

### Approach

- **Reverse engineering and process understanding:** reviewed the existing VBA-based workflow and traced data movements, transformations, dependencies and downstream uses in the production environment.
- **Technical documentation:** documented the end-to-end process and modelled key interactions and structures using UML use-case, sequence and class diagrams.
- **Progressive delivery:** prepared a roadmap to organise the migration into stages, track progress, obtain feedback and validate deliverables incrementally.
- **Migration to Python:** progressively replaced the macro-based processing with a Python application connected to the Data Warehouse. The application automated ETL operations and formatted structured outputs to meet developers' requirements.
- **Reliability and execution:** implemented non-regression tests to check that the migrated processing remained consistent, and packaged the application with Docker so the team could run it in its environment.

### Engineering practices demonstrated

Legacy-system understanding · Data-flow mapping · Technical documentation · UML modelling · Incremental delivery · Python ETL · Regression testing · Docker

## 2. Predictive analysis of mobile-offer sales drivers

### Business question

The second workstream focused on analysing factors associated with changes in mobile-offer sales volumes and giving business teams a way to explore different commercial assumptions.

One example was examining how a change in the commissions paid to partners could relate to a change in sales volumes.

### Approach and deliverable

- Analysed commercial data to study the determinants associated with changes in mobile-offer sales volumes.
- Developed a predictive-analysis approach to explore relationships between explanatory variables and sales indicators.
- Built a Streamlit interface through which business users could configure their analysis, choose the KPIs they wanted to examine and adjust relevant scenario parameters.
- Enabled users to modify assumptions — including partner commission levels — and observe the corresponding changes in predicted sales volumes and selected indicators.

### Business value

The interface made quantitative analysis more accessible to non-technical users. Rather than requiring them to manipulate code or datasets, it provided a configurable way to explore commercial scenarios and support data-informed discussions.

**Interpretation note:** scenario outputs are model-based predictions under specified assumptions. They should not be interpreted as proof of a causal effect unless supported by a separate causal-identification strategy.

## Skills illustrated

| Area | Skills |
|---|---|
| Data engineering | Python, ETL, Data Warehouse integration, data transformation |
| Software and delivery | VBA-to-Python migration, UML, technical documentation, roadmap, Docker |
| Data quality | Non-regression testing, progressive validation |
| Data science | Exploratory analysis, predictive modelling, scenario analysis |
| Business-facing tools | Streamlit, KPI configuration, decision support |

## Confidentiality

The examples above are intentionally described without internal data, source code, customer information, confidential performance figures or sensitive implementation details. The case study is intended to explain the nature of my contribution, not to reproduce Bouygues Telecom's internal systems.

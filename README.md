# Animal Shelter Adoption Analysis

## Live Dashboard

**View the interactive Tableau dashboard here:**

👉 [Animal Shelter Adoption Analysis Dashboard](https://public.tableau.com/app/profile/lisa.bentman/viz/animal-shelter-adoption-analysis/AnimalShelter)


## Project Overview

This project analyses the animal adoption journey for a fictional animal shelter, from initial enquiry through to adoption and return outcomes.

The objective was to identify factors influencing adoption success, understand where potential adopters drop out of the process, and provide recommendations to improve adoption rates and reduce returns.

The analysis follows a consultancy-style approach, combining data cleaning, exploratory analysis and business recommendations.

## Business Objectives

This analysis aimed to answer the following questions:

- Where do potential adopters drop out of the adoption process?
- Which enquiry channels generate the most successful adoptions?
- How do animal characteristics influence adoption outcomes?
- Does adopter engagement impact adoption success?
- What factors contribute to animal returns?

## Dataset

The project uses four datasets representing different stages of the adoption journey:

<img width="993" height="550" alt="datasets" src="https://github.com/user-attachments/assets/5a942c26-76b8-4e8a-832c-b65658330008" />

### Final Dataset

**Enquiries:** 320

**Visits:** 270

**Successful Adoptions:** 105

## Data Cleaning & Preparations

Key cleaning activities included:

- Standardising species, health status and enquiry channels
- Resolving duplicate adoption records
- Validating enquiry → visit → adoption timelines
- Handling missing and inconsistent values
- Creating customer journey metrics
- Engineering features such as:
- Age bands
- Response time bands
- Adoption journey durations
- Visit attendance metrics
  
## Analysis Performed

### Adoption Funnel Analysis

Investigated conversion rates across the adoption journey:

Enquiry → Visit → Adoption

### Channel Performance

Compared adoption volumes and conversion rates across:

- Website
- Facebook
- Email
- Phone
- Walk-In

### Animal Characteristics

Explored adoption outcomes by:

- Species
- Age
- Health Status
- Colour
- Sex

### Engagement Analysis

Investigated relationships between:

- Response times
- Number of visits
- Adoption success

### Return Analysis

Explored characteristics associated with returned animals.

## Key Findings

**1. The largest drop-off occurs between visit and adoption**
- 84.4% of enquiries progressed to a visit.
- Only 38.9% of visits resulted in adoption.
- Overall enquiry-to-adoption conversion was 32.8%.</br>

<img width="1285" height="153" alt="adoption_funnel" src="https://github.com/user-attachments/assets/e190f6ca-ebe9-421c-8339-81632e39dec6" />

**2. Website enquiries drive adoption success**
- Website generated 57 successful adoptions.
- Facebook achieved a higher conversion rate (40%).
- Website results were more reliable due to significantly larger volumes.</br>

<img width="419" height="834" alt="channel_performance" src="https://github.com/user-attachments/assets/a7d99f41-e989-4364-9bc7-9d910b8217ea" />

**3. Animals in good health account for most successful adoptions**
- 62 successful adoptions involved animals in good health.
- Adoption volumes declined across other health categories.</br>

<img width="1486" height="137" alt="health_status" src="https://github.com/user-attachments/assets/981f6713-7be4-40f6-99d2-15c4f0018d79" />

**4. Most successful adoptions occur after a single visit**
- One attended visit resulted in 83 successful adoptions.
- Higher conversion rates for multiple visits were driven by small sample sizes.</br>

<img width="352" height="719" alt="visit_summary" src="https://github.com/user-attachments/assets/3ce08a11-3f14-4e1c-9af1-fa18d0e88c48" />

**5. Rapid responses appear beneficial**
- Most successful adoptions originated from enquiries responded to within 24 hours.
- Longer response times were associated with lower adoption volumes.</br>


## Business Recommendations

1. Improve post-visit follow-up processes to increase visit-to-adoption conversion.
2. Continue prioritising website acquisition while monitoring Facebook as a potential growth channel.
3. Target enquiry response times within 24 hours.
4. Increase visibility of animals with health challenges through focused marketing campaigns.

## Deliverables

### Visualisations

The Tableau dashboard focuses on four key business questions:

- **Adoption Funnel:** Where are potential adopters dropping out?
- **Channel Performance:** Which channels drive successful adoptions?
- **Health Status:** Which health groups account for successful adoptions?
- **Visit Summary:** Does increased engagement improve adoption outcomes?

[Tableau Public Dashboard](https://public.tableau.com/app/profile/lisa.bentman/viz/animal-shelter-adoption-analysis/AnimalShelter)

<img width="1192" height="793" alt="tableau_dashboard" src="https://github.com/user-attachments/assets/849569d8-56e6-4cd0-bf4d-2bf3b6a67dc0" />

### Analysis

| File | Description |
|--------|--------|
| [01_data_preparation.ipynb](notebooks/01_data_preparation.ipynb) | Data cleaning and preparation |
| [02_analysis_and_insights.ipynb](notebooks/02_eda_and_insights.ipynb) | Exploratory analysis and business insights |

### Presentation

[animal-shelter-slide-deck.pdf](slides/animal-shelter-slide-deck.pdf)

## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook
- Tableau Public
- GitHub

## Analytical Considerations

Throughout the analysis, percentage-based findings were validated against underlying population counts to avoid drawing conclusions from small sample sizes. Several apparent patterns (e.g. Facebook adoption rates, adoption outcomes after three visits, and unknown health statuses) were investigated further before being incorporated into recommendations.

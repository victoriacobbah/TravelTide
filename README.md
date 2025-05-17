# TravelTide: Personalised Rewards Segmentation

This repository documents a full data analytics project for TravelTide — a fictional travel booking platform aiming to improve customer retention via personalised rewards.

The project supports a marketing strategy led by Elena Tarrant, the fictional Head of Marketing, to assign targeted perks such as free hotel meals, checked bags, cancellation fee waivers, exclusive discounts, or bonus hotel nights.

## Project Goal
To segment TravelTide users based on their demographics and behaviour, and assign each segment a personalised reward that increases loyalty and retention.

## Tools Used
**Python (Pandas, NumPy) – Data analysis and cleaning**

**PostgreSQL – Data extraction and session-level feature engineering**

**Tableau – Visualisation and dashboard creation**

**Colab – Project workbook (hosted in TravelTide_Final_Workbook.ipynb)**

**PowerPoint / Canva – Final presentation**

## Methodology

**Cohort Selection**
- Focused on high-engagement users (8+ sessions since 4 Jan 2023)  
- Justified through exploratory session analysis  

**Session-Level Dataset**
- Joined users, sessions, hotels, and flights  
- Engineered features like trip duration, hotel spend, discount responsiveness  

**User-Level Aggregation**
- Created features per user: trip frequency, spend, booking patterns, etc.  

**Segmentation**
- Used a structured rule-based decision tree, rather than clustering  
- Groups defined by life stage (e.g. Solo Parent) and refined by behaviour  

**Perk Assignment**
- Each segment matched with a reward aligned to its needs and value  

**Churn Risk & Priority Score**
- Churn score based on recency of activity  
- Priority score = churn risk × total spend  
- Segments ranked by total priority score to support marketing targeting
.


## Final Segments
| Segment                        | Assigned Perk                         |
|-------------------------------|----------------------------------------|
| Family Traveller              | Free Night with Flight Booking         |
| Business Solo                 | Upgrade to Business Class              |
| Luxury Solo Traveller         | Lounge Access                          |
| Couple Explorer               | Free Room Upgrade                      |
| Independent Explorer          | Late Check-Out                         |
| Bargain Hunter                | Early Access to Exclusive Deals        |
| Luxury Couple Selective Booker | Free Hotel Meal                       |
| Solo Parent Traveller         | 10% off Next Hotel Booking             |
| Couple City Breaker           | Free Hotel Breakfast                   |
| Detached Family Traveller     | Free Checked Bag                       |
| Unconverted User              | 15% off Next Booking                   |


## Outcome
- Identified 11 behavioural segments aligned to marketing needs

- Assigned perks based on value, responsiveness, and cost-effectiveness

- Segments prioritised for campaign testing using a churn-weighted score

- Decision tree logic can be applied to future users or legacy data

## Files Included
- TravelTide_Final_Workbook.ipynb – Full Colab project

- travel_tide_session_level_cohort.csv – Session level data of selected cohort

- travel_tide_segmented_users.csv – Final export of enriched user data

- Traveltide Presentation.pptx – Slides for stakeholder communication

- README.md – This document

## Notes
This project was completed as part of a data analytics training programme. All data is fictional and created for educational use.

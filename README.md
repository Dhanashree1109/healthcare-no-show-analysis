\# Reducing Patient No-Show Rates – Healthcare Analytics Project



\## Business Problem

Approximately 20% of scheduled appointments result in no-shows, reducing provider utilization, disrupting scheduling workflows, and impacting operational efficiency.



\## Objective

Identify key drivers of appointment no-shows and develop a simple risk segmentation framework to enable targeted intervention strategies.



---



\## Dataset

\- 110,000+ appointment records

\- Multi-specialty hospital scheduling data

\- Features include demographic, clinical, scheduling, and reminder information



---



\## Data Preparation

\- Standardized column names

\- Converted scheduling timestamps to datetime

\- Engineered `lead\_time\_days`

\- Removed logically invalid negative lead times

\- Removed invalid age records

\- Created binary `no\_show\_flag` (1 = No-show)



---



\## Key Findings



\### 1. Lead Time is the Strongest Driver

No-show risk increases significantly with scheduling delay:

\- 0–1 days: 6.6%

\- 30+ days: 33.0%



\### 2. Younger Patients Have Higher Risk

Patients aged 18–35 show ~23.8% no-show rate compared to ~15–16% among older patients.



\### 3. SMS Reminders Reduce Risk for Long Lead Times

While aggregate analysis suggested higher no-show rates among SMS recipients, stratified analysis showed a 6–7 percentage point reduction for appointments scheduled 15+ days in advance.



\### 4. Rule-Based Risk Segmentation

A simple operational rule:

\- Lead time > 14 days

\- Age < 35

\- No chronic condition



Identified a cohort with:

\- 37.7% no-show rate vs 17.9% baseline



---



\## Business Recommendations

\- Implement targeted reminder escalation for high-risk segment

\- Apply controlled overbooking for long lead-time slots

\- Introduce 48-hour confirmation workflow for flagged patients



---



\## Tools Used

\- Python

\- Pandas

\- Matplotlib

\- Jupyter Notebook



---



\## Outcome

Developed an actionable risk segmentation framework enabling data-driven intervention strategies to improve provider utilization.


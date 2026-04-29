# Migrant Deaths Along the U.S.-Mexico Border: A Data Analysis

A Malloy data analysis project investigating migrant death patterns across the
entire U.S.-Mexico border using the No More Deaths Border Death Database. This
project explores 8,832 recorded deaths spanning 44 years and surfaces concrete
insights intended to support humanitarian search efforts and broader awareness
of one of the most significant ongoing humanitarian crises in the United States.

---

## Overview

The No More Deaths Border Death Database compiles records of recovered migrant
remains across the southern U.S. border from 2002 to 2025, drawing on data from
ten different county medical examiner offices, sheriff's departments, and Border
Patrol records. After standardizing and combining the data into one master
dataset, this analysis revealed geographic, temporal, and demographic patterns
that point to the scale of the crisis and the gaps in identification that
remain a challenge for families, researchers, and humanitarian organizations.

---

## The Story

### A Recorded Increase Over the Past Two Decades

![Deaths by Year](images/deaths_by_year.png)

The dataset spans from 1981 to early 2025, and the most notable trend is the
sustained increase in recorded deaths beginning in the early 2000s, with a
secondary surge in the past five years. The highest year on record was 2022
with 683 deaths, followed by 2023 with 646 and 2021 with 630. Early 2025 has
already recorded 68 deaths in the first few months alone.

![Recent Surge](images/recent_surge.png)

### Geographic Distribution

![Deaths by State](images/deaths_by_state.png)

Arizona accounts for 4,636 of the 8,832 recorded deaths in this dataset,
followed by Texas with 3,037 and California with 799. Pima County Arizona
alone is responsible for 3,377 deaths once both spellings of the county name
are combined, making it the single county with the highest concentration of
recorded deaths in the dataset.

### Causes of Death

![Causes of Death](images/deaths_by_cause.png)

The two most common findings in the dataset are nearly tied: 1,569 deaths
attributed to environmental exposure and 1,567 cases recorded only as skeletal
remains. The skeletal remains figure is significant, as it indicates that
those remains were recovered long after death, often making timely
identification difficult or impossible. Together, exposure and skeletal
remains account for over 35 percent of all recorded deaths in the dataset.

### Demographic Distribution

![Deaths by Nationality](images/deaths_by_nationality.png)

Mexican nationals account for the largest portion of identified decedents at
1,430, followed by Guatemala with 346, Honduras with 228, and El Salvador
with 205. Several other countries across Central and South America are also
represented in the dataset.

---

## The Identification Gap

One of the most significant findings of this analysis is how often basic
information about decedents is unknown. Of the 8,832 recorded deaths, only
4,881 had a known age at time of death, meaning 45 percent of all decedents
could not be identified to the level of even establishing an approximate age.
While 7,324 cases (83 percent) do have GPS coordinates recorded, those
coordinates often mark a recovery location rather than a death site, and the
interval between death and recovery can extend into months or years.

---

## What I Learned

What surprised me most about this project was the scope of the identification
gap. Going into this analysis I expected that some records would be incomplete,
but I did not expect that nearly half of all recorded deaths would have
unknown ages, or that skeletal remains would account for nearly the same
number of cases as environmental exposure itself. These findings together
illustrate the challenges of recovery and identification along remote
stretches of the border.

What was harder than expected was navigating the inconsistencies in the source
data. The original Excel file contained 13 separate sheets, each with
different column structures, formats, and conventions. Some county records
were detailed and standardized, while others were sparse or used non-numeric
entries like "Est. 17" or "Unknown" in fields meant for ages. Cleaning and
standardizing this data into one usable master file required several rounds
of error handling and manual mapping, but the result is a dataset that can
now be queried freely in Malloy and used to surface meaningful insights.

---

## Sample Insight

A query of the counties with the highest recorded death counts shows that
Pima County Arizona accounts for the largest concentration of cases in the
entire dataset, with over 3,300 records when accounting for variations in
capitalization. This concentration aligns with the most extreme stretches of
the Sonoran Desert, where summer temperatures regularly exceed 110 degrees
Fahrenheit and where humanitarian organizations like Humane Borders and No
More Deaths maintain water stations and conduct search and recovery
operations.

---

## How to Run This Analysis

1. Clone this repository:

    git clone https://github.com/dprieto-robles/border-deaths-malloy.git

2. Open the project folder in VS Code with the Malloy extension installed

3. Open the `border_deaths.malloy` file

4. Run any of the views by clicking the play button above any `run:` statement

---

## Who Would Care

This dataset and analysis is intended to support several audiences. Search
and recovery organizations can use the geographic concentrations and location
data to focus their efforts where recorded deaths are most clustered.
Humanitarian aid groups can use the cause-of-death patterns to inform where
water drops and emergency supplies may be most useful. Journalists and
researchers can use the temporal trends to better understand how border death
data has evolved over the past four decades. Families searching for missing
loved ones may find ongoing identification work documented and trackable
through datasets like this one. As of February 2026, 1,653 decedents in
Arizona alone remain unidentified, which highlights the continued importance
of this work.

---

## Data Source

This analysis is built on the No More Deaths Border Death Database, which
compiles data from county medical examiner offices, sheriff's departments,
and Border Patrol records across the southern U.S. border. The original
dataset is available at nomoredeaths.org and represents one of the most
comprehensive public records of recovered migrant remains currently available.

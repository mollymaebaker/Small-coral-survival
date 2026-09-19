# Marine heatwaves reshape survival of small corals, revealing size- and taxa-specific vulnerabilities

## Overview
This repository provides survival data for over 3,000 small coral colonies (<10 cm) across multiple eastern Indian Ocean reefs (Ningaloo, Mermaid, Scott and Ashmore reefs), taxa (mostly Acropora, Isopora, Pocillopora, Goniastrea and Porites), sizes (0.3 - 10 cm) and levels of heat stress and bleaching (background conditions, a moderate bleaching event, and severe bleaching event).

These data were analysed, and the results were presented in the paper 'Marine heatwaves reshape survival of small corals, revealing size- and taxa-specific vulnerabilities.'

We strongly recommend reading the paper before using this repository. The knowledge gaps adressed in this paper and the key findings are summarised in the following schematic:

<img width="4409" height="2484" alt="Paper coms" src="https://github.com/user-attachments/assets/2ba39f09-2a09-4d21-9cb5-da13728c9e79" />

## Repository structure

### /data

In the 'data' folder you will find seperate csv files for each reef and montioring period including:

1) 'Ningaloo_smallcoral_survival.csv'

   Monitoring duration: ~1 year
   
   Montioring dates: June/August 2023 - August 2024
   
   Taxa: Acroporiidae, Pocilloporiidae and Merulinidae
   
   Level of heat stress: background conditions (i.e., no significant heat stress occured during the monitoring period, DHW<4).
   
2) 'Mermaid_T1_smallcoral_survival.csv'
   
   Monitoring duration: 1 year
   
   Montioring dates: October 2023 - October 2024
   
   Taxa: Acropora spp., Isopora spp., Pocillopora spp., Goniastrea spp. and Porties spp.
   
   Level of heat stress: background conditions

3) 'Scott_smallcoral_survival.csv'
   
   Monitoring duration: ~1 year
   
   Montioring dates: 2006-2007, 2007-2008, 2008-2009 (i.e., three one year monitoring periods).
   
   Taxa: Acropora spicifera (2006-2009) and Goniastrea spp. (only monitored from 2008-2009)
   
   Level of heat stress: background conditions

4) 'Ashmore_smallcoral_survival.csv'
   
   Monitoring duration: ~1 year
   
   Montioring dates: April 2024 - March 2025
   
   Taxa: Acropora spp., Isopora spp., Pocillopora spp., Goniastrea spp. and Porties spp.
   
   Level of heat stress: moderate bleaching event
   
5) 'Mermaid_T2_smallcoral_survival.csv'
   
   Monitoring duration: 6 months
   
   Montioring dates: October 2024 - April 2025
   
   Taxa: Acropora spp., Isopora spp., Pocillopora spp., Goniastrea spp. and Porties spp.
   
   Level of heat stress: severe bleaching event
   
Each csv file contains the following columns:
- Date: The date the colony was first tagged (initial survey / baseline).
- Site: Reef site where the colony was tagged.
- Plot: Plot number within a site.
- Tag: Physical tag identifier within a plot.
- ID: Unique identifier for colonies surrounding each tag.
- Size_x: Maximum diameter (cm) at the beginning of the monitoring period (T1_Size_x for Mermaid T2).
- T1_Date OR T2_Date: Date of re-survey.
- T1_Survival OR T2_Survival: Survival outcome of each resurvey (1 = survived, died = 0).
- Taxa OR Taxa_broad: Coral taxa.
- Site_Plot: Nested spatial grouping variable (Site + Plot combined). Useful for Bayesian hierarchical modelling.

NOTE: Rather date columns the 'Scott_postrecrutiment_survival.csv' has the column 'year' which represents the montioring period e.g., 6-7 corresponds to 2006-2007.


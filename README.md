# Visual Analytics Midterm Project
## This repo is about the Tableau Workbook for Fall '24 Visual Analytics Course

### Introduction
 The dashboard would be utilized by healthcare workers to get a quick overview of the most current observation values from collecting vitals to lab reports while also seeing past trends to compare them to what may be the patient's normal or if values are getting better or worsening. 


### Data:
- Due to the sensitive nature of EHR's, synthetic data created through [Synthea](https://synthetichealth.github.io/synthea/) was utilized. mCODE released data created using Synthea to produce 10 year EHR records for oncology paitents. Only a single record was used from the download due to me still being new to the world of HIT and Interoperability making working with FHIR JSON bundles being a little hard to understand parsing wise to flatten it into a familiar format of CSV and tableau struggled as well to interpret them. To overcome this issue, a Python Library 

### Future Work: 
- As I gain more experiance working with FHIR bundles, working to integrate the ability to view more paitents at once to get either a full view of what a hospitals floor demographics and health look like or so a nurse can get a view of more of their patients easily.
- Add colors to values that may be high or low to quickly highlight areas of concern. For example with labs, if the patients have a value of 9 g/dL for their hemoglobin, then highlight the value in red. 


[Link to Project Workbook](https://public.tableau.com/app/profile/nicole.anderson8589/viz/MidtermProject_17298390741440/SummaryDash?publish=yes)

[mCODE EHR Test Data](https://confluence.hl7.org/display/COD/mCODE+Test+Data)



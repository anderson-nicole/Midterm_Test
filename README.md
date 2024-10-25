# Visual Analytics Midterm Project
## This repo is about the Tableau Workbook for Fall '24 Visual Analytics Course

### Introduction
- The dashboard is a visual summary of a patient's EHR observations, specifically here their vitals and blood test lab results. The use case is for a healthcare professional auch as a doctor or nurse be able to quickly visualize a paitents current status along with what trends the paitent has to better understand the results of the lab or assess what is normal for a patients vitals.
  
### Data:
- Due to the sensitive nature of EHR's, synthetic data created through [Synthea](https://synthetichealth.github.io/synthea/) was utilized. [mCODE released data](https://confluence.hl7.org/display/COD/mCODE+Test+Data) created using Synthea to produce 10 year EHR records for oncology paitents. Only a single record was used from the download due to me still being new to the world of HIT and Interoperability making working with FHIR JSON bundles being a little hard to understand parsing wise to flatten it into a familiar format of CSV and tableau struggled as well to interpret them. To overcome this issue, a Python Library [Fhiry](https://github.com/dermatologist/fhiry?tab=readme-ov-file) was used to read in and convert the data into a Pandas dataframe that I could then export as a CSV. 

### Future Work: 
- As I gain more experiance working with FHIR bundles and play around with other FHIR parsers, I would like to integrate the ability to view more paitents at once to get either a full view of what a hospitals floor demographics and health look like or so a nurse can get a view of more of their patients easily. This also would allow for more variety of visuals rather than just line plots for trends. 
- Add colors to values that may be high or low to quickly highlight areas of concern. For example with labs, if the patients have a value of 9 g/dL for their hemoglobin, then highlight the value in red. 

[Link to Project Workbook](https://public.tableau.com/app/profile/nicole.anderson8589/viz/MidtermProject_17298390741440/SummaryDash?publish=yes)

[mCODE EHR Test Data](https://confluence.hl7.org/display/COD/mCODE+Test+Data)
- 'Adriene242_Lang846_41fc105e-fdbc-6483-55d7-beceb378f456.json' was the file used from the folder. 



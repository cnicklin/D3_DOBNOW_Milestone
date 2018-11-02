## DOB NOW: Build Milestones

The New York City Department of Buildings (DOB) DOB NOW Build Milestones application displays basic details for selected DOB NOW Build filings on an interactive map of New York City. Each filing is represented as a dot on the map, and clicking the dot or the item on the list below brings you to a profile page that shows major milestone dates for that filing. The application is updated daily with the latest filings for Antenna, Curb Cut, Fence, Plumbing, Scaffold, Sidewalk Shed, Sign, Sprinkler, and Standpipe filings in DOB NOW.

![Milestone Map Page](https://github.com/cnicklin/D3_DOBNOW_Milestone/blob/gh-pages/MapPage.PNG)

## Data Source

Data flows from the BI tool to GitHub public hold. This is a daily automated process. It creates results in 2 formats: JSON (for search) and CSV (for map imaging).

<img align="center" width="" height="" src="https://github.com/cnicklin/D3_DOBNOW_Milestone/blob/gh-pages/Flow.PNG" alt="Milestone App Flow Diagram">

## Data Definitions
Definitions for elements on the Profile Page are listed below, but can also be viewed by hovering over the field name on the webpage.

### Profile Page

| Field Name | Definition |
|-------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Job Number | The unique ID number assigned when the applicant submits the filing to the Department of Buildings. |
| BIN Number | The Building Identification Number assigned by the Department of City Planning. |
| Work Type | The type of work described in this filing. It could include plumbing, sprinkler, construction fence, or another type of work. |
| Job Type | This indicates the extent of the work being done. NB means a new building is being built. A1 means that extensive alterations will be done resulting in a change of building occupancy. A2 means that alterations will be done but will not result in a change of building occupancy. A3 indicates that minor alterations will be done. |
| Professional Certification | Yes indicates that the applicant is certifying that the work being performed complies with all applicable laws and codes. This job will then skip review by a plan examiner. |
| Filing Status | The current status of the filing. A definition for each of the values for Filing Status can be found on our [Status Glossary](https://github.com/cnicklin/D3_DOBNOW_Milestone/blob/gh-pages/Statuses.md). |
| Number of Resubmissions | During review, the Department of Buildings may return a filing to the applicant multiple times because the information is incomplete, because it needs correction, or another reason. This indicates the total number of times the filing was resubmitted, and does not include the initial submission. |
| Job Description | The general description of the work being applied for. This field is free text, and is filled out by the applicant. |

### Milestone Dates

| Field Name | Definition |
|-------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Filing Date | The date that the applicant submitted the filing to the Department of Buildings. |
| CPE Assigned Date | The date that the filing was assigned to a Chief Plan Examiner for review or for delegation to a Plan Examiner. |
| CPE Action Date | The date that the Chief Plan Examiner took action on the filing. |
| PE Assigned Date | The date that the filing was assigned to a Plan Examiner. |
| First Objection Date | The date that the filing was first returned to the applicant with objections. A filing may go through several cycles of being submitted, reviewed by a Plan Examiner, and returned to the applicant with objections. A filing may never receive objections and therefore may skip this milestone date. |
| Latest Objection Date | The most recent date that the filing was returned to the applicant with objections. A filing may never receive objections and therefore may skip this milestone date. |
| Latest Resubmit Date | The most recent date that the filing was resubmitted to the Department of Buildings for review. A filing may never be sent back to the applicant and therefore may skip this milestone date. |
| QA Supervisor Assigned Date | The date that the filing was assigned to a QA Supervisor for review or for delegation to a QA Admin. |
| QA Admin Assigned Date | The date that the filing was assigned to a QA Admin. |
| Initial QA Failed Date | The first date that the filing was returned to the applicant because it was incomplete or needed correction. A filing can fail QA multiple times, or it may be approved on the first review and skip this milestone date. |
| Plan Approved Date | The date that the filing was approved. The applicant can now pull permits. |
| Initial Permit Issued Date | The first date that a permit was issued. Multiple permits can be issued for a job filing. |
| Latest Permit Expiration Date | The expiration date for the most recent permit. Multiple permits can be issued for a job filing. |
| Permit Signed Off Date | The date that the Department of Buildings signed off that the work was completed. |

## Built With

* [R](https://www.r-project.org/)
    + Core packages(dplyr, tidyr, RJDBC, ...)
* [Carto VL](https://carto.com/developers/carto-vl/)
* [Mapbox GL](https://www.mapbox.com/mapbox-gl-js/api/)
* [D3](https://d3js.org/)
* [Bootstrap](https://getbootstrap.com/)

## Built by

* [DOB Analytics and Data Science Team](https://www1.nyc.gov/site/buildings/about/metrics-reports.page) - If you have questions or feedback, comment here on github or email us at [Analytics@buildings.nyc.gov](mailto:analytics@buildings.nyc.gov). (Note: We're hiring a [web developer](https://a127-jobs.nyc.gov/psc/nycjobs/EMPLOYEE/HRMS/c/HRS_HRAM.HRS_APP_SCHJOB.GBL?Page=HRS_APP_JBPST&Action=U&FOCUS=Applicant&SiteId=1&JobOpeningId=373170&PostingSeq=1)!)

## Acknowledgments

* Inspired by [NYC Planning Labs](https://planninglabs.nyc/)


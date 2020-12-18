# SolarElectricAnalysis
Solar_Electric_Programs_Reported_by_NYSERDA__Beginning_2000.<br/>
UB EAS 503 Final project.<br/>

# Goal of Project
To predict the 2025 Solar KW DC capacity whether it meets the Goal of NY State.

# Contributors
## Ayush Gandhi ayushgan@buffalo.edu.<br/>
## Mark Sigalov marksiga@buffalo.edu.<br/>
## Raj Karra rajyavar@buffalo.edu.<br/>

# Introduction
Notebook link : https://github.com/ayushga1194/SolarElectricAnalysis/blob/main/SolarAnalysis_NYSERDA_Final.ipynb<br/>
Time Period of the dateset is 2000-2020
The data was extracted from New York State Data Portal
Dataset contains total of 113K records.<br/>
The data set used for analysis is from year 2000-2020.

Dataset Information:- https://data.ny.gov/Energy-Environment/Solar-Electric-Programs-Reported-by-NYSERDA-Beginn/3x8r-34rs

# Solar Data
| Data Label | Data Type | Data Description
| :------ |:------ | :------ |
| Project Number | Text | Unique identifier for project |
| City | Text | Name of city for project location |
| County | Text | Name of county for project location |
| Zip Code | Text | Zip code for project location |
| Sector | Text | Name of project sector. The sectors in this dataset are either Residential or Non-Residential |
| Program Type | Text | Name of program type; either Residential/Small Commercial, Commercial/Industrial (Competitive), or Commercial/Industrial (MW Block) |
| Solicitation | Text | NYSERDA Program Opportunity Notification (PON) or Request for Proposal (RFP) number |
| Electric Utility | Text | Name of electric utility for project location |
| Purchase Type | Text | Solar photovoltaic project purchase agreement type. The purchase types are either Lease, Purchase or Power Purchase Agreement. Blank cells represent data that were not required or are not currently available |
| Date Application Received | Date | Date project application was received by the program |
| Date Completed | Date | Date NYSERDA recognized the project as interconnected and operational, and closed out the project application. Blank cells represent pipeline data for projects not yet completed |
| Project Status | Text | Either Complete or Pipeline. Complete indicates projects that are interconnected and operational, and closed out the project application. Pipeline indicates projects with an active application that are not yet complete. Pipeline projects are subject to change |
| Contractor | Text | Name of entity responsible for installation of the project. Blank cells represent data that were not required or are not currently available. Contractor data is not provided for Pipeline projects, except for Community Distributed Generation projects. |
| Primary Inverter Manufacturer | Text | Name of primary inverter manufacturer for project. Some projects may use more than one type of inverter manufacturer. Only the primary inverter manufacturer is provided. Blank cells represent data that were not required or are not currently available |
| Primary Inverter Model Number | Text | Name of primary inverter model number for project. Some projects may use more than one type of inverter model. Only the primary inverter model number is provided. Blank cells represent data that were not required or are not currently available |
| Total Inverter Quantity | Numeric | Quantity of all inverters installed for project. Quantity provided is for all inverters, not just the primary inverter. Blank cells represent data that were not required or are not currently available |
| Primary PV Module Manufacturer | Text | Name of primary photovoltaic (PV) module manufacturer for project. Some projects may use more than one type of PV module manufacturer. Only the primary PV module manufacturer is provided. Blank cells represent data that were not required or are not currently available |
| Primary PV Module Model Number | Text | Name of primary photovoltaic (PV) module model number for project. Some projects may use more than one type of PV module model. Only the primary PV module model number is provided. Blank cells represent data that were not required or are not currently available |
| Total PV Module Quantity | Numeric | Quantity of all photovoltaic (PV) modules installed for project. Quantity provided is for all PV modules, not just the primary PV module. Blank cells represent data that were not required or are not currently available |
| Project Cost | Currency | Cost of project in US dollars (USD). Blank cells represent data that were not required or are not currently available |
| $Incentive | Currency | Amount of project incentives paid by the program in USD. Blank cells represent data that were not required or are not currently available. Projects that received Green Jobs-Green NY financing but no incentive show an Incentive Amount of $0 |
| Total Nameplate kWDC | Numeric | The sum of kilowatt (kW) DC capacity ratings of the installed photovoltaic modules |
| Expected kWh Annual Production | Numeric | Expected annual electricity production in kilowatt- hours (kWh) as a result of project |
| Remote Net Metering | Text | Indicates if project is Remote Net Metered. Blank cells represent data that were not required or are not currently available |
| Affordable Solar | Text | Indicates if project is part of Affordable Solar program  |
| Community Distributed Generation | Text | Indicates if project Community Distributed Generation (Shared Solar) |
| Green Jobs Green New York Participant | Text | Indicates if project accessed Green Jobs-Green New York financing. Blank cells represent data that were not required or are not currently available |

# Data Cleansing
### Following columns were dropped from dataset
-  Reporting Period
-  Legacy Project Number
-  State
-  Solicitation
-  Primary Inverter Model Number
-  PV Module Model Number
-  Primary Inverter Model Number
-  Primary Inverter Model Number

### After data cleansing the final data set has 112K records of solar power plants

# Derived Columns
- Days- Difference of DateApplicationReceived and DateApplicationCompleted

# Clinical Data Models

Open Medical Record System ([OpenMRS](https://openmrs.org/)): is an open-source electronic health record (EHR) system designed to support the delivery of healthcare in resource-constrained environments.

**Open source Research Common Data Models:**
- i2b2: Harvard University / Partners Healthcare
- OMOP: OHDSI Consortium
- Sentinel: USA FDA
- PCORnet: Patient Centered Outcomes Research Institute

The Observational Medical Outcomes Partnership ([OMOP](https://www.ohdsi.org/data-standardization/#:~:text=The%20Observational%20Medical%20Outcomes%20Partnership,that%20can%20produce%20reliable%20evidence.)) Common Data Model (CDM) is an open community data standard, designed to standardize the structure and content of observational data and to enable efficient analyses that can produce reliable evidence.

i2b2 is an open-source clinical data warehousing and analytics research platform, which enables sharing, integration, standardization, and analysis of heterogenous data from healthcare and research.

[Sentinel Common Data Model (SCDM)](https://www.sentinelinitiative.org/methods-data-tools/sentinel-common-data-model): a standard data structure that allows Data Partners to quickly execute distributed programs against local data.

[MIMIC-III](https://physionet.org/content/mimiciii/1.4/) (‘Medical Information Mart for Intensive Care’) is a large, single-center database comprising information relating to patients admitted to critical care units at a large tertiary care hospital. 

**Extraction, Transformation, and Loading (ETL)**
- Data profiling: Understanding the features of the data in a source database
- Data mapping: Moving data from source location to target location
- Terminology mapping: Converting codes/values used in source to codes/values allowed in target
  
[White Rabbit data](https://github.com/OHDSI/WhiteRabbit)


## ICD-coding

Hierarchical condition category (HCC) coding helps communicate **patient complexity** and paint a picture of the whole patient. In addition to helping predict health care resource utilization, RAF scores are used to risk adjust quality and cost metrics. By accounting for differences in **patient complexity, quality and cost performance** can be more appropriately measured. 

icd-mappings: This tool helps working with ICD codes. It maps between ICD versions (such as between **ICD9 and ICD10**). Also maps to other codings such as CCS (Computer Software Classification), and CCI (Chronic Condition Indicator). 

Icdcodex: A python library for building vector representations of ICD-9 and ICD-10 codes. Because it takes advantage of the hierarchical nature of ICD codes, it also provides these hierarchies in a **networkx** format.

Example: Predicting MIMIC-III diagnostic codes: [get the data.csv in Google Cloud BigQuery](https://mimic.mit.edu/docs/gettingstarted/cloud/bigquery/)

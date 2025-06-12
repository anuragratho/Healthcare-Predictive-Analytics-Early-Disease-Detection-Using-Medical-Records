# Healthcare-Predictive-Analytics-Early-Disease-Detection-Using-Medical-Records

# Project Objectives
These were the four subsystemic goals of this research project with an overreaching aim of promoting distributed computing in healthcare analytics. The primary technical goal was to develop a big data pipeline using MapReduce paradigm of Hadoop and fine-tune them to suit characteristic of medical data ingestion, computation and storage. Based on such foundation, the project achieved further clinical goals of establishing methods of analytical nature to estimate frequencies of symptoms and analyze possible trends in patient manifestations with emphasis placed on normalization and statistical verification. The last integration problem was solvedthrough the creation of data pipelines for transfer of data from HDFS storage to MySQL DBs; there was a challenge in mapping the schema as well as the integrity of data between different structures of storage. Last, the project created a version controlled and parameterized structure with clear explanation for all methods used and sufficient documentation to allow for validation for the framework and scales to the larger clinical datasets. To achieve these aims, it included quantifiable results such as processing speed and accuracy, confidence intervals for certain types of clinical data, methods for system integration, and principles of reproducibility – all of which were developed to form a quantifiable approach to analyzing medical data that meets both short term research demands as well as long term requirements in the medical industry.

# Research Questions
The study was focused on the following three research
questions:
1. Technical Implementation: What are the
effective patterns for dividing the medical
record data for analysis using Hadoop
MapReduce design, setting up jobs and
performance enhancing techniques?
2. System Architecture: How should distributed
computing components be architecturally
integrated with traditional database systems
to maintain data consistency while enabling
analytical flexibility?
3. Clinical Insights: What quantitative patterns
emerge from distributed processing of
symptom data, and how do these findings
compare with established medical knowledge
about symptom prevalence?

# Dataset Description
The project utilized a structured dataset of patient medical records containing five key attributes. PatientID served as the unique identifier for each record, while Age documented patient age in years. Gender recorded biological sex using binary classification. The Symptoms field captured patient- reported health complaints as text entries, and Diagnosis contained the physician's clinical assessment. While the initial dataset contained only six records for development purposes, the schema was designed to accommodate scaling to thousands of records without structural modification. This way, this limited dataset size let to check IF this architecture could really work out while being sure that it will be
scalable to a more typical for healthcare practice amount of data.

# Data Processing Pipeline
The presented workflow is divided into four subprocesses from the analysis point of view. The first activity required taking the records which are in CSV format and then loading them into the Hadoop Distributed File System using the commands in terminal. After ingestion, the core MapReduce process launched a custom Java application, which contained the mapper and/or reducer functionalities. The last activity called database integration involved putting the processed results into a MySQL relational database. Last of all, the last data analysis stage used scripts written in Python language to compute other insights from the summarized data using statistical and graphical analysis.

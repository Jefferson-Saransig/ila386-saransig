# Open Science Conventions


## 1. File and variable naming

I will use descriptive and consistent names for files, variables, and R objects. 
I will use the same variable names across datasets when they refer to the same information, 
such as participant, word, origin, and genre. 
I will use the template [glottocode]_[date]_[participant]_[session] for recordings, 
for example qvi_2026-07-17_p01_s01.wav. 
I will use leading zeros for participant and session numbers, such as p01 and s01, 
and three digit record IDs such as 001, 002, and 003.

For R objects, I will use prefixes to distinguish different types of objects. 
I will use data_ for datasets, fig_ for figures, tbl_ for tables, and 
fml_ for models. 
When possible, I will use names that correspond to the files they represent, 
such as data_raw for a raw dataset and data_clean for a cleaned dataset. 
I will use NA to represent missing data.


## 2. Folder and project structure
I will follow the following structure:

project_name/ 
├── data/ 
├── src/ 
├── results/ 
├── doc/ 
└── README.md

I will use data/ for raw data and metadata, 
src/ for R scripts and other project source code, 
results/ for files generated during data cleaning and analysis, and 
doc/ for documents such as notes and paper drafts.
## 3. README
I am not really sure what to include here but I assume it is something that other researchers 
can read in case they want to replicate the experiment or study. So, my README file 
would describe the purpose of the project, the data, and the organization of the 
files. It will explain what each main folder contains and provide basic information 
about how to reproduce the analysis when applicable.

## 4. Raw and processed data

I will keep raw data separate from processed data. 
Original audio and video recordings will be preserved without modification, 
while cleaned transcriptions, datasets, and other files generated during analysis will be 
stored separately. 
I will document important changes made during data processing and use 
scripts whenever possible so that processed data can be traced back to the original data.


## 5. Data dictionary

record_id: integer (type), none (units), 3-digit numbers (coding), NA (missing)
participant: character (type), none (units), p-01 (coding), NA (missing)
word: character (type), none (units), word transcribed (coding), NA (missing)
origin: categorical (type), none (units), kichwa, Spanish, other (coding), NA (missing)
genre: categorical (type), none (units), narrative, conversation (coding), NA (missing)


## 6. Code and script organization
I will keep project code in the src/ directory and organize scripts according to their 
main purpose. For example, I will use separate scripts for data cleaning, analysis, and 
generating tables or figures. 
I think the names should be short and understandable such as clean_data and analyze_borrowing
## 7. Version control
I will follow what we have been doing in class: 
meaningful change-> review-> commit-> descriptive message-> upload
## 8. Data and code sharing
For the audio files, I will archive them in an language archive such as AILLA. 
To share my codes I think I can use GitHub and have it public and published once a paper
is published
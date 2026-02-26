# Code repository for the analysis of the study 'A common neural mechanism underlies experiences of passage of time'

### Scripts:
  - **MNE Python**
    - ***environment.yml***<br/>
      File that allows recreating the virtual environement with the packages and version numbers necessary to run the scripts.<br/><br/>
    - ***sfct.eeg_preprocessing_subjectwise.ipynb***<br/>
      Jupyter Notebook script for eeg preprocessing of individual subjects<br/><br/>
    - ***sfct.eeg_preprocessing_groupwise.ipynb***<br/>
      Jupyter Notebook script that combines data from all subjects after they were preprocessed individually ('sfct.eeg_preprocessing_subjectwise.ipynb')<br/><br/>
    - ***sfct.eeg_analysis_basic.ipynb***<br/>
      Jupyter Notebook script for basic description of EEG signal and face validity checks<br/><br/> 
    - ***sfct.eeg_analysis_ML.ipynb***<br/>
      Jupyter Notebook script that performs the machine learning analysis and saves subject and groupwise results<br/><br/>
  - **R**

    - ***sfct.data_preparation.Rmd***<br/>
      RMarkdown script for preparing data for R anayssis<br/>
    - ***sfct.eeg_analysis.Rmd***<br/>
      RMarkdown script for descriptive statistics and statistical anaylsis of behavioral and ML results<br/>
    - ***sfct.eeg_analysis_suppl.Rmd***<br/>
      RMarkdown script for creating supplementary material for analyses<br/><br/>


### How to use:
  - Copy raw data (OpenNeuro repository ds007454) to foler data/bids_dataset<br/>
  - Save data directory path as 'path_study_data' in *.ipynb scripts and as 'dir.data' in *.Rmd scripts<br/>
  - anaylsis scripts require file 'feature_and_ratings.group.csv' created by script 1b 

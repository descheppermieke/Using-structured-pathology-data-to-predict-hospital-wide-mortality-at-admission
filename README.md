# Using-structured-pathology-data-to-predict-hospital-wide-mortality-at-admission

In this repository you can find the data that belongs to the article:

Using structured pathology data to predict hospital-wide mortality at admission
Authors: M. Deschepper, W. Waegeman, D. Vogelaers, K. Eeckloo



## Datasets for ICD-10 models

- ds_icd10_admission: dataset with all ICD-10 diagnoses known at admission
- ds_icd10_admission_wo: dataset with all ICD-10 diagnoses known at admission WITHOUT DNR or palliative care codes
- ds_icd10_discharge: dataset with all ICD-10 diagnoses known at discharge
- ds_icd10_discharge_wo: dataset with all ICD-10 diagnoses known at discharge WITHOUT DNR or palliative care codes
- ds_icd10_admission_woPD: dataset with all ICD-10 diagnoses known at admission WITHOUT the principal diagnosis
- ds_icd10_discharge_woPD: dataset with all ICD-10 diagnoses known at discharge WITHOUT the principal diagnosis
- ds_icd10_admission_wo_woPD: dataset with all ICD-10 diagnoses known at admission WITHOUT DNR or palliative care codes and WITHOUT the principal diagnosis
- ds_icd10_discharge_wo_woPD: dataset with all ICD-10 diagnoses known at discharge WITHOUT DNR or palliative care codes and WITHOUT the principal diagnosis

All datasets have the following columns:

- outcome: the outcome variable (survivor = 0, non-survivor = 1)
- diaghoofdstukXX: binary variable for diagnosis chapter XX
- diagcatXX: binary variable for the diagnosis category XX
- diagnosisXX: binary variable for the diagnosis XX


## Datasets for RoM models

- ds_rom_admission: dataset with the 4 Risk of Mortality Categories as calculated with the diagnosis known at admission
- ds_rom_discharge: dataset with the 4 Risk of Mortality Categories as calculated with the diagnosis known at discharge
- ds_rom_admission_wo: dataset with the 4 Risk of Mortality Categories as calculated with the diagnosis known at admission WITHOUT DNR or palliative care codes
- ds_rom_discharge_wo: dataset with the 4 Risk of Mortality Categories as calculated with the diagnosis known at discharge WITHOUT DNR or palliative care codes

All datasets have the following columns:
- outcome: the outcome variable (survivor = 0, non-survivor = 1)
- rom1: binary variable Risk of Mortality Category 1
- rom2: binary variable Risk of Mortality Category 2
- rom3: binary variable Risk of Mortality Category 3
- rom4: binary variable Risk of Mortality Category 4

Every record can only have 1 RoM.

## Datasets for CCI models

- ds_cci_admission: dataset with the Charlson Comorbidity Score as calculated with the diagnosis known at admission
- ds_cci_discharge: dataset with the Charlson Comorbidity Score as calculated with the diagnosis known at discharge
- ds_cci_admission_wo: dataset with the Charlson Comorbidity Score as calculated with the diagnosis known at admission WITHOUT DNR or palliative care codes
- ds_cci_discharge_wo: dataset with the Charlson Comorbidity Score as calculated with the diagnosis known at discharge WITHOUT DNR or palliative care codes

All datasets have the following columns:
- outcome: the outcome variable (survivor = 0, non-survivor = 1)
- cci: numeric Charlson Comorbity Score 

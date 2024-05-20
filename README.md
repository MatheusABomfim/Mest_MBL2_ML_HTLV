# Qualifica-o_ML_HTLV
Codes in Python, to implementation of diverse models of Machine Learning, trying to promote prognosis in People Living with HTLV

Divided into three documents:
- The first involved data pre-processing and model evaluation with default parameters
- The second involved optimizing hyperparameters
- And in the third, application of Explainable AI (XAI) methods 

##**Notes/reminders:**

* Clinical data has been excluded
(because they will still be extracted from the medical records, classifying the oligosymptomatic patients separately, allowing a better evaluation of the machine)

* This script is based on the file: "Based on the ML Wine data set" with the appropriate modifications.

* It uses only one machine-learning evaluation model, several of which will be used in the final master's work. The current script corresponds to a training script developed in conjunction with pacific (more complex).

## Dictionary:
* In column: SEX
 * M = 0
 * F = 1

* In column: HAM/TSP
* No myelopathy = 0
* HAM/TSP = 1

# **Categorized data_1:**
named as = cat_data_1

Creation of a new data table, transforming the binary variables referring to urinary dysfunctions into categorical numerical variables, exclusion of uninformative columns and categorization of pain subtypes. Including the conversion of "Hipereflexia" and "Hiperflexia em MMII", como somente "Hipereflexia.

Dictionary:
- Urinary_symptoms:
 - Polyuria: 1 +
 - Neurogenic bladder: 2 +
 - Neurogenic bladder + urinary incontinence:3
 - Nocturia: 4 +
 - Nocturia + urinary incontinence: 5
 - Dysuria: 6
 - Dysuria + neurogenic bladder: 7

- Pain:
 - non-specific pain: 1
 - joint pain: 2
 - lower back pain: 3
 - lower limb pain: 4
 - lower limb pain + other site of pain: 5

- Weakenes:
 - normal levels of strength: 0
 - weakness or lost of stregth: 1

- Wandering:
 - normal walking: 0
 - abnormal walking: 1

At this point, df is the new data set with the change in the selected characteristics

# **Categorized data_2:**
named as = cat_data_2

- Urinary_symptoms:
 - Polyuria: 1 +
 - Neurogenic bladder: 2 +
 - Neurogenic bladder + urinary incontinence:3
 - Nocturia: 4 +
 - Nocturia + urinary incontinence: 5
 - Dysuria: 6
 - Dysuria + neurogenic bladder: 7

- Pain:
 - non-specific pain: 1
 - joint pain: 2
 - lower back pain: 3
 - lower limb pain: 4
 - lower limb pain + other site of pain: 5

- Weakenes:
 - normal levels of strength: 0
 - weakness or lost of stregth: 1

- Wandering:
 - normal walking: 0
 - abnormal walking: 1

- Chronic diseases:

The presence of any of the following variables resulted in the dataset being converted to 1:
 - diabetes
 - obesity
 - diabetes
 - osteoporosis
 - chronic kidney disease
 - Hypothyroidism
 - arthrosis
 - hypertension
 - arthrosis/ diabetes/hypertension
 - arthrosis/diabetes/hypertension

- Mental disorders:
The presence of any of the following variables resulted in the dataset being converted to 1:
 - psychotic breaks/compulsive crises
 - insomnia
 - outbreaks/insomnia/crisis
 - schizophrenia
 - anxiety
 - psychiatric illness
 - anxiety/depression
 - depression


- Neurological disorder/symptoms:
The presence of any of the following variables resulted in the dataset being converted to 1:
 - Paresthesia
 - Weakness
 - Numbness
 - Hypermotility

- The presence of any of the following variables resulted in the dataset being converted to 2:
 - Paresis
 - Hypereflexia
 - Spasticity
 - Gait (related to locomotion problems)

In the event of the presence of the above-mentioned symptoms associated with the disorders, the sample was converted into 2


#**Categorized data_3:**
named as = cat_data_3

- Urinary_symptoms:
 - Polyuria: 1 +
 - Neurogenic bladder: 2 +
 - Neurogenic bladder + urinary incontinence:3
 - Nocturia: 4 +
 - Nocturia + urinary incontinence: 5
 - Dysuria: 6
 - Dysuria + neurogenic bladder: 7

- Pain:
 - non-specific pain: 1
 - joint pain: 2
 - lower back pain: 3
 - lower limb pain: 4
 - lower limb pain + other site of pain: 5

- Weakenes:
 - normal levels of strength: 0
 - weakness or lost of stregth: 1

- Wandering:
 - normal walking: 0
 - abnormal walking: 1
Use of a wheelchair included difficulty walking

- Mental disorders:
The presence of any of the following variables caused the data set to be converted into the respective numbers described below:
 - psychotic breaks/compulsive crises: 1
 - insomnia: 2
 - outbreak/insomnia/crisis: 3
 - schizophrenia: 4
 - anxiety: 5
 - psychiatric illness: 6
 - anxiety/depression: 7
 - depression : 8

- Neurological disorder/symptoms:
The presence of any of the following variables caused the data set to be converted into the respective numbers described below:
 - Paresthesia: 1
 - Paresis: 2
 - Hypereflexia: 3
 - Paresthesia/hypereflexia: 4
 - Weakness: 5
 - Weakness/paresthesia: 6
 - Weakness/paresis: 7
 - Numbness: 8
 - Spasticity: 9
 - Hypereflexia/spasticity or gait: 10
 - Paresis/spasticity or gait: 11
 - Loss of strength: 12
 - Loss of strength/paresthesia: 13
 - Loss of strength/paresis/spasticity or gait: 14
 - Hypermotility: 15
 - Paresthesia/hyperreflexia/hypermotricity: 16
 - Weakness: 17
 - Weakness/hypereflexia: 18

- Chronic diseases:
 - Diabetes: 1
 - Obesity: 2
 - Diabetes/Obesity: 3
 - Osteoporosis: 4
 - Chronic kidney disease: 5
 - Hypothyroidism: 6
 - Arthrosis: 7
 - Arthrosis/diabetes: 8
 - Hypertension: 9
 - Arthrosis/diabetes/hypertension: 10
 - Arthrosis/diabetes/hypertension: 11



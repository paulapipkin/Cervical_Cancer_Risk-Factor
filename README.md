
# Cervical Cancer Risk

By **Paula Pipkin** 

### Evaluating Cervical Cancer Risk :

This dataset focuses on the prediction of indicators/diagnosis of cervical cancer. 
The features cover demographic information, habits, and historic medical records.


### Data:

The data set source is the website UCI Machine Learning Repository and here is a link to the original data:
[https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/](https://archive.ics.uci.edu/ml/datasets/Cervical+cancer+%28Risk+Factors%29#)

## Methods

- After some pre cleaning, two copies of the data were made so EDA could be done without risking leakage.  
- EDA was used to show correlations between some relevant features
- 3 models were applied, Random Forrest, KNN and Lgbm


## Results

LGBM had the best results and it was the model chosen to be used.

### EDA

#### Patients with HPV
![sample image](plot1.png)

> Out of 835 patients, 1/3 or 33% of those patients diagnosed with HPV were also diagnosed with cervical cancer, only 5% of those without HPV were diagnosed with Cervical Cancer.

> "Virtually all cervical cancers are caused by HPV. Routine screening can prevent most cervical cancers by allowing health care providers to find and remove precancerous cells before they develop into cancer." (source: https://www.cancer.gov/about-cancer/causes-prevention/risk/infectious-agents#hpv).

#### Hormonal Contraceptives Use

![sample image](plot2.png)

> In our sample, 18% more women were diagnosed with Cervical Cancer among those patients using Hormonal Contraceptive for longer than 10 years.

> The longer a woman uses oral contraceptives, the greater the increase in her risk of cervical cancer. One study found a 10% increased risk for less than 5 years of use, a 60% increased risk with 5–9 years of use, and a doubling of the risk with 10 or more years of use (source: https://www.cancer.gov/about-cancer/causes-prevention/risk/hormones/oral-contraceptives-fact-sheet)

### Metrics

#### Scores and Confusion Matrix:

Accuracy 0.96

| Score        | Classe 0                   | Classe 1       |
| ------------- | -----------------------| -------- |
| Precision | 0.98	 | 0.69 |
| Recall |0.97             |0.79  |


![sample image](confusionmatrix.jpg)

## Recommendations, Limitations & Next Steps:

- For this case, a false posite and a false negative are very serious errors, a patient without cancer should not be subimitted to treatment, and a positive result can't go untreated.
- Having that in mind, I still believe that our model is useful, however I would suggest that a second measure would be used to confirm the results prior to treatment or dismissal of treatment.

### For further information


For any additional questions, please contact **paulareche@gmail.com**

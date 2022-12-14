# <p align = "center"> Adult's Income Prediction </p>

This data was extracted from the 1994 Census bureau database by Ronny Kohavi and Barry Becker (Data Mining and Visualization, Silicon Graphics). A set of reasonably clean records was extracted using the following conditions: ((AAGE>16) && (AGI>100) && (AFNLWGT>1) && (HRSWK>0)). <br>
The prediction task is to determine whether a person makes over $50K a year.

## DATA DEFINATION

The Adult's Income dataset is collected from kaggle using this <a href = "https://www.kaggle.com/uciml/adult-census-income"> https://www.kaggle.com/uciml/adult-census-income. </a> <br>
This dataset has 48842 rows × 15 columns. <br>

1. age: continuous.
2. workclass: Private, Self-emp-not-inc, Self-emp-inc, Federal-gov, Local-gov, State-gov, Without-pay, Never-worked.
3. fnlwgt: continuous.
4. education: Bachelors, Some-college, 11th, HS-grad, Prof-school, Assoc-acdm, Assoc-voc, 9th, 7th-8th, 12th, Masters, 1st-4th, 10th, Doctorate, 5th-6th, Preschool.
5. education-num: continuous.
6. marital-status: Married-civ-spouse, Divorced, Never-married, Separated, Widowed, Married-spouse-absent, Married-AF-spouse.
7. occupation: Tech-support, Craft-repair, Other-service, Sales, Exec-managerial, Prof-specialty, Handlers-cleaners, Machine-op-inspct, Adm-clerical, Farming-fishing, Transport-moving, Priv-house-serv, Protective-serv, Armed-Forces.
8. relationship: Wife, Own-child, Husband, Not-in-family, Other-relative, Unmarried.
9. race: White, Asian-Pac-Islander, Amer-Indian-Eskimo, Other, Black.
10. sex: Female, Male.
11. capital-gain: continuous.
12. capital-loss: continuous.
13. hours-per-week: continuous.
14. native-country: United-States, Cambodia, England, Puerto-Rico, Canada, Germany, Outlying-US(Guam-USVI-etc), India, Japan, Greece, South, China, Cuba, Iran, Honduras, Philippines, Italy, Poland, Jamaica, Vietnam, Mexico, Portugal, Ireland, France, Dominican-Republic, Laos, Ecuador, Taiwan, Haiti, Columbia, Hungary, Guatemala, Nicaragua, Scotland, Thailand, Yugoslavia, El-Salvador, Trinadad&Tobago, Peru, Hong, Holand-Netherlands.

## METHODS
In this project, we have employed the following steps:

1. Data Collection
2. Data Cleaning
3. Data Analysis
4. Data Preprocessing(Preparation)
5. Model Training
6. Performance Evaluation

We have implemented the following models: <br>

1. SVM
2. Logistic Regression
3. Naive Bayes

## PERFORMANCE EVALUATION
We have calculated the performance by calculating `Precision`, `Recall` , `True positive/negative` for all the models and built a `Confusion Matrix` for the same.

## RESULTS
1. Gender Distribution based on Income

![gender](https://user-images.githubusercontent.com/39597515/209453637-16edd869-0883-46b5-be5f-9deb5ef920bf.png)

2. Education Count 

![Education_Count](https://user-images.githubusercontent.com/39597515/209453649-4297145c-b7d1-4b9d-b14f-7699ded9b131.png)

3. Age Vs Marital Status

![AgeVsMarital_Status](https://user-images.githubusercontent.com/39597515/209453655-7032160b-1d9d-4f6d-8137-a6a893ef4295.png)

## MODEL EVALUTATION
Here is the tabular view of `Accuracy` and `Time taken` to run the model - 

| Model  | Accuracy | Time |
| ------------- | ------------- | ------------- | 
| Logistic Reg - Oversampled  | 83.2% | 824.2s |
| Logistic Reg - Undersampled  | 82.5% | 102.9s |
| Logistic Reg - SMOTE | 83.7% | 848s | 
| SVM - Oversampled  | 83% | 303.9s |
| SVM - Undersampled  | 81% | 22.89s |
| SVM - SMOTE | 84% | 300.4s |
| Naive Bayes - Oversampled  | 76% | 23.41s |
| Naive Bayes - Undersampled  | 76% | 3.69s |
| Naive Bayes - SMOTE | 85% | 23.67s |

## CONCLUSION

1. Only a few of the traits are closely associated to income projection, according to the correlation table. <br>
2. The choice of such columns has a big impact on the model's accuracy. Random Forest is also the best fit for this dataset. Males have a higher rate of incorrect predictions than females. <br>
3. The dataset does not have to be perfect or small all of the time. As a result, we must define a method, a method that can be applied to every dataset. <br>
4. Here is a step-by-step explanation of the workflow, which you may apply to your own dataset. <br>
5. Also, different types of visualizations effectively portray data based on a combination of attribute types (numerical, categorical) and a classification technique that is totally reliant on the dataset.

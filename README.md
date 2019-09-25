# Random Forest Medical Cost Estimation
My [Medical Cost EDA](https://github.com/namas191297/medical_cost_eda) repository consists the exploratory data analysis and the visualization of the medical record data in the ```insurance.csv``` file. 

This repository consists of the python notebook in which I have built a Random Forest Regressor used to predict and estimate the medical cost that a person may incur given certain attributes and features. All the features are listed in the aforementioned repository. 

## Random Forests

Random forests or random decision forests are an ensemble learning method for classification, regression and other tasks that operates by constructing a multitude of decision trees at training time and outputting the class that is the mode of the classes or mean prediction of the individual trees

![Random_Forest](https://miro.medium.com/max/592/1*i0o8mjFfCn-uD79-F1Cqkw.png)




## Estimation Features

Based on the EDA of the given data, the correlation between the independent features and the medical cost revealed all features except the ```region``` attribute play a role in estimating the medical costs, the features that are used are :

* age: age of primary beneficiary

* sex: insurance contractor gender, female, male

* bmi: Body mass index, providing an understanding of body, weights that are relatively high or low relative to height, objective index of body weight (kg / m ^ 2) using the ratio of height to weight, ideally 18.5 to 24.9

* children: Number of children covered by health insurance / Number of dependents

* smoker: Whether a person smokes or not



## Categorical to Nominal Transformation

In order to include certain categorical features in the model, it was necessary to convert them from a categorical type to nominal type so that numpy was able to interpret them and take them as input into the model.

These categorical features and their nominal interpretation is:

* Sex - [0 - Female, 1 - Male]
* Smoker - [0 - No, 1 - Yes]
* Region - [0 - Northeast, 1 - Northwest, 2 - Southeast, 3 - Southwest]

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
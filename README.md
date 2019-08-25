# Classifying Bitcoin Ponzi Schemes with Machine Learning

## Overview
The invention of cryptocurrencies has created new opportunities for criminals to leverage variety of traditional scam techniques. Fraudulent activity associated with cryptocurrency is experiencing explosive growth and is a significant barrier for widespread adoption of blockchain technology.

In 2018, losses from cryptocurrency-related crimes amounted to US$1.7 billion. Cryptocurrency fraudsters rely on tried-and-true Ponzi schemes that use income from new participants to pay out returns to earlier investors. Early detection of ponzi schemes in this domain using machine learning can save hundreds of millions of dollars.

## Dataset
Dataset is available at [seanconeys/Bitcoin_Ponzi_ml](https://github.com/seanconeys/Bitcoin_Ponzi_ml/) repository.<br>
Source: [Link](https://raw.githubusercontent.com/seanconeys/Bitcoin_Ponzi_ml/master/datasets/final_aggregated_dataset.csv)

The authors of the dataset collected data associated with ponzi schemes from several forums that advertised "high yield investment programs" disguised as ponzi schemes. Some of these sites include [bitcoinwhoswho.com](https://bitcoinwhoswho.com), [bitcointalk.org](https://bitcointalk.org), and [reddit.com](https://reddit.com). The other class of non-ponzi schemes were derived from this [study](https://arxiv.org/pdf/1803.00646.pdf).

## Dependencies
* numpy
* pandas
* matplotlib
* seaborn
* scikit-learn
* xgboost

## Result
|Model   |AUC   |
|---|---|
|Logistic Regression   |0.62   |
|SVM   |0.80   |
|Random Forest   |0.88   |
|XGBoost   |0.94   |

### Logistic Regression
![Logistic Regression](https://raw.githubusercontent.com/prabodhw96/Bitcoin-Ponzi/master/images/lr_auc.png)

### SVM
![SVM](https://raw.githubusercontent.com/prabodhw96/Bitcoin-Ponzi/master/images/svm_auc.png)

### Random Forest
![Random Forest](https://raw.githubusercontent.com/prabodhw96/Bitcoin-Ponzi/master/images/rf_auc.png)

### XGBoost
![XGBoost](https://raw.githubusercontent.com/prabodhw96/Bitcoin-Ponzi/master/images/xgb_auc.png)
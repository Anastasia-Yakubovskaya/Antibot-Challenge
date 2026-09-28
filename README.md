# Antibot-Challenge
A machine learning solution for detecting bots from user behavior and event history.

A solution for detecting bots based on user behavior and event history.

## What the model does

The code:

* processes user events;
* builds time-based and sequential features;
* uses information about items, search queries, and User-Agent;
* takes previous user activity into account;
* trains several models and combines their predictions.

The main models are **LightGBM, CatBoost, and XGBoost**.

## Validation

Because the data has a temporal structure, the model is validated using previous days to predict later days.

The main metric is:

**Precision at Recall >= 0.70.**

## Result

Best score on the hidden test set:

```text
Precision@Recall>=0.70 = 0.85302
```

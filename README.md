# Brain Stroke Prediction using XGBoost and Neural-Network
## Introduction
A stroke is a medical condition in which poor blood flow to the brain causes cell death.
### Dataset
- The dataset is obtained from [Kaggle](https://www.kaggle.com/datasets/zzettrkalpakbal/full-filled-brain-stroke-dataset?datasetId=2343381&sortBy=voteCount).
### Context
- There are two main types of stroke: ischemic, due to lack of blood flow, and hemorrhagic, due to bleeding. Both cause parts of the brain to stop functioning properly. 
- Signs and symptoms of a stroke may include an inability to move or feel on one side of the body, problems understanding or speaking, dizziness, or loss of vision to one side. Signs and symptoms often appear soon after the stroke has occurred. 
- If symptoms last less than one or two hours, the stroke is a transient ischemic attack (TIA), also called a mini-stroke. A hemorrhagic stroke may also be associated with a severe headache. The symptoms of a stroke can be permanent. Long-term complications may include pneumonia and loss of bladder control.
- The main risk factor for stroke is high blood pressure. Other risk factors include high blood cholesterol, tobacco smoking, obesity, diabetes mellitus, a previous TIA, end-stage kidney disease, and atrial fibrillation.

## Conclusion

**AUC-PR:** The Neural Network model has a slightly higher AUC-PR score (0.1906) compared to the XGBoost model (0.1545). AUC-PR measures the area under the precision-recall curve and provides an aggregate measure of model performance for imbalanced datasets.

**Precision and Recall:** Both models have high precision and recall for class 0 (no stroke), indicating that they are good at identifying instances of no stroke correctly. However, both models perform poorly for class 1 (stroke), with low precision, recall, and F1-score. This suggests that the models struggle to correctly classify instances of stroke.

**F1-score:** The F1-scores for both classes are low for both models, indicating poor overall performance in capturing the true positive instances for both strokes and no strokes.

**Accuracy:** Both models have the same accuracy of 0.93, which might be misleading due to the class imbalance. High accuracy can be achieved by simply predicting the majority class (no stroke) most of the time.

Overall, both models show suboptimal performance in accurately predicting instances of stroke, as evidenced by low precision, recall, and F1-score for class 1. However, the Neural Network model slightly outperforms the XGBoost model in terms of AUC-PR.

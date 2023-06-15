# Machine Learning to Predict the Development of Atrial Fibrillation in Critically Ill Patients

This is the repository for our recent project that uses machine learning to predict atrial fibrillation in critically ill patients. We used data from the Medical Information Mart for Intensive Care (MIMIC-IV) database. The model achieved an area under the receiver operator characteristic curve (AUC) of 0.850. A compact model using 15 features in addition to 2 newly engineered features achieved a comparable AUC of 0.820.

<p align="center">
  <img src="https://github.com/laithomari/machine_learning_afib_prediction/assets/54318618/d601a780-033e-4b13-b95a-4940b7089796.png" width="600" height="500" />
</p>

The newly added features were the following:

1. **Older septic**: a categorical feature indicating if the patient is 70 years old or older and is septic.
2. **Cardiac risk score**: a score that incorporates patient's preexisting cardiac related risk factors:

<p align="center">
  <img src="https://github.com/laithomari/machine_learning_afib_prediction/assets/54318618/4627f18c-c775-462a-93fd-8552476fd6cc.png" />
</p>

Based on the Shapley Additive exPlanations (SHAP) analysis, the two newly engineered features, _older septic_ and _cardiac risk score_, were the second and third most influential features on model performance, respectively.

<p align="center">
  <img src="https://github.com/laithomari/machine_learning_afib_prediction/assets/54318618/eebfa8c4-1456-4e0d-80a6-27e0c550067c.png" width="600" height="622" />
</p>

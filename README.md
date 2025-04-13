# Synapse 2k25 🚀

# Clone the repository
```bash
git clone https://github.com/yourusername/conversion-uplift-modeling.git
```


# Run the notebook
jupyter notebook model_pipeline.ipynb

**Overview** 🔍
This project focuses on understanding and modeling the drivers behind conversion (purchase/target action) using advanced machine learning and uplift modeling techniques. The aim is to not only predict conversions but also identify the causal impact of treatment/exposure and provide explainable insights into which features influence user behavior.

**Key Components**
💡 Uplift Modeling: Implemented SoloModel and TwoModel strategies to capture incremental lift in conversions due to exposure (e.g., marketing campaigns). Helps identify users who are more likely to convert when treated.

⚖️ Imbalanced Classification Handling:

Undersampled majority class for a more balanced representation.

Used StratifiedKFold with logistic regression and gradient boosting models.

Evaluated using Recall, Precision, AUC, and Confusion Matrix.

📈 Model Explainability with SHAP:

Generated SHAP value plots to interpret model predictions.

Visualized feature-level impact and global importance.


**Visual Insights (SHAP Plots)** 📊
Below are sample SHAP plots from the model trained on the validation set:

![Screenshot 2025-04-13 223017](https://github.com/user-attachments/assets/81bf602c-cc9b-4b31-bd21-bb92ae2ad39e)
SHAP feature analysis through Xg Boost, suggesting **f4** as the most important feature.

![Screenshot 2025-04-13 223028](https://github.com/user-attachments/assets/b0a2ccee-4505-42fb-9185-085713e68f96)
SHAP feature analysis through Gradient Boost, suggesting **f10** as the most important feature.

![Screenshot 2025-04-13 223035](https://github.com/user-attachments/assets/f81e0626-0100-4e21-8194-37aff5499234)
SHAP feature analysis through Logistic Regression, suggesting **f4** as the most important feature.

**Uplift curve** 📊
![Screenshot 2025-04-13 225215](https://github.com/user-attachments/assets/e6623cb3-e72f-4631-924b-5c01749ad46f)

By: Shourya Aggarwal
Refer to the report in Conversion attribution.pdf

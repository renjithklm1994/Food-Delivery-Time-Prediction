

## 🧠 Machine Learning Model

We used a **Logistic Regression** model to classify whether a delivery will be **on time (1)** or **delayed (0)**.

### 🔍 Features Used:
- `Traffic_Conditions`
- `Weather_Conditions`
- `Delivery_Person_Experience`
- `Distance_feature`
- `Order_Time`
- `Rush_hour`

###  Target Variable:
- Binary classification:
  - `0` → Delayed
  - `1` → On Time

---

## Model Performance

### Accuracy
```
0.5375
```

### Confusion Matrix
```
           Predicted
           0     1
Actual  0 [26,  10]
        1 [27,  17]
```

###  Classification Report
| Class | Precision | Recall | F1-score | Support |
|-------|-----------|--------|----------|---------|
| 0 (Delayed)   | 0.49 | 0.72 | 0.58 | 36 |
| 1 (On Time)   | 0.63 | 0.39 | 0.48 | 44 |

- **Macro F1-score:** 0.53  
- **Weighted F1-score:** 0.53

---

## Model Coefficients

| Feature | Coefficient |
|---------|-------------|
| Intercept | -0.6396 |
| Traffic_Conditions | -0.0266 |
| Weather_Conditions | -0.1597 |
| Delivery_Person_Experience | 0.4992 |
| Distance_feature | 0.8092 |
| Order_Time | 0.0640 |
| Rush_hour | 0.0203 |

---

##  Observations

- **Distance** and **delivery person experience** have the strongest positive influence on on-time deliveries.
- The model performs better at predicting delayed orders (recall = 0.72) than on-time ones (recall = 0.39).
- Overall accuracy is moderate (53.75%) and could be improved.




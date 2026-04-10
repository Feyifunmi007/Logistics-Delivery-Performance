# 🚚 Delivery Performance Analysis

## 📌 Project Overview
This project analyzes delivery operations to identify key factors influencing delivery success, delays, failures, and cost efficiency. Using regression analysis and descriptive statistics, the study provides data-driven insights to support logistics planning and operational decision-making.

---

## 🎯 Research Questions
The project answers the following business questions:

1. Which delivery partner has the highest success rate?  
2. Which vehicle type is most cost-efficient relative to:
   - Distance  
   - Package weight  
3. Which region has the highest delivery success, failures, and delays?  
4. How do weather conditions affect delivery success, failure, and delay?  
5. What effect does weather have on delivery cost?  

---

## 📊 Key Findings

- **Delivery Partner Performance:**  
  FedEx recorded the highest delivery success rate.

- **Cost Drivers:**  
  Delivery cost is driven by:
  - Distance (₦4.99 per km)  
  - Package weight (₦2.95 per kg)  
  Vehicle type is not a significant predictor.

- **Regional Performance:**  
  - West → Highest delivery success and failures  
  - Central → Highest delays  

- **Impact of Weather:**  
  - Rainy weather increases delays and failures  
  - Clear and hot weather improve delivery success  

- **Weather vs Cost:**  
  Weather conditions do not significantly affect delivery cost.

---

## 📈 Methodology

- Data Cleaning  
- Descriptive Statistics  
- Multiple Regression Analysis  

---

## 📉 Regression Analysis Results

### 1. Delivery Cost Model (Distance, Weight, Vehicle Type)

| Variable        | Coefficient | Significance |
|----------------|------------|--------------|
| Intercept      | (Constant) | — |
| Distance       | 4.99       | Significant (p < 0.001) |
| Weight         | 2.95       | Significant (p < 0.001) |
| Vehicle Type   | ~0         | Not Significant (p > 0.05) |

**Model Summary:**
- R² = 0.991  
- F-statistic = 396,474 (p < 0.001)  

**Interpretation:**  
The regression model shows that delivery cost is strongly explained by distance and package weight, accounting for 99.1% of the variation in cost. Specifically, each additional kilometer increases delivery cost by approximately ₦4.99, while each additional kilogram increases cost by ₦2.95. Vehicle type was not statistically significant, indicating that it does not meaningfully influence cost when distance and weight are controlled for. This implies that pricing decisions should focus primarily on distance and package weight rather than vehicle category.

---

### 2. Weather Impact on Delivery Outcomes

| Weather Condition | Effect on Success | Effect on Delay | Effect on Failure |
|------------------|------------------|-----------------|-------------------|
| Rainy            | Decreases        | Increases       | Increases         |
| Foggy            | Slight impact    | Slight increase | Minimal           |
| Clear/Hot        | Increases        | Decreases       | Decreases         |

**Interpretation:**  
Weather conditions significantly affect delivery performance. Adverse conditions, particularly rain, reduce delivery success and increase both delays and failures. In contrast, favorable weather conditions improve delivery efficiency.

---

### 3. Weather Impact on Delivery Cost

| Metric        | Value |
|--------------|------|
| R²           | 0.00005 |
| F-statistic  | 0.257 |
| p-value      | 0.937 |

**Interpretation:**  
The regression results indicate that weather conditions do not significantly influence delivery cost. The model explains almost none of the variation in cost, suggesting that pricing is independent of weather and driven by operational variables such as distance and weight.

---

## 🛠️ Tools & Technologies

- Microsoft Excel  
- Regression Analysis  
- Statistical Techniques  

---

## 📁 Project Structure

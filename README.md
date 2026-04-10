# 🚚 Delivery Performance Analysis

![Image](https://github.com/user-attachments/assets/32d87f2d-0f3a-4337-aa2f-7b6b9e3b04a8)

## 📌 Project Overview
This project analyzes delivery operations to identify key factors influencing delivery success, delays, failures, and cost efficiency. Using regression analysis and descriptive statistics, the study provides data-driven insights to support logistics planning and operational decision-making.

---

## 🎯 Objectives
The project answers the following business questions:

1. Which delivery partner has the highest success rate?  
2. Which vehicle type is most cost-efficient relative to distance and package weight?  
3. Which region has the highest delivery success, failures, and delays?  
4. How do weather conditions affect delivery success, delay, and failure?  
5. What effect does weather have on delivery cost?  

---

## 📊 Key Findings

- **FedEx** has the highest delivery success rate  
- Delivery cost is driven by **distance and package weight**, not vehicle type  
- **West region** → highest success & failures | **Central** → highest delays  
- **Rainy weather worsens performance**, while **clear/hot weather improves it**  
- Weather does **not affect delivery cost**

---

## 📈 Methodology

- Data Cleaning  
- Descriptive Statistics  
- Multiple Regression Analysis  

---

## 📉 Regression Analysis Results

### 1. Delivery Cost Model

| Variable      | Coefficient | Significance |
|--------------|------------|--------------|
| Distance     | 4.99       | Significant (p < 0.001) |
| Weight       | 2.95       | Significant (p < 0.001) |
| Vehicle Type | ~0         | Not Significant |

**Model Summary:**  
R² = 0.991 | F = 396,474 (p < 0.001)

**Interpretation:**  
Delivery cost is strongly explained by distance and package weight. Vehicle type does not significantly influence cost, meaning pricing decisions should focus on logistics variables rather than transport mode.

---

## 🌦️ Weather Impact on Delivery Outcomes

### (a) Delivery Success Model

| Variable | Coefficient | P-value | Interpretation |
|----------|------------|--------|----------------|
| Intercept | 0.7121 | 0.000 | Base success rate |
| Foggy | -0.0152 | 0.0649 | Not significant |
| Rainy | -0.0856 | <0.001 | Significant decrease |
| Hot | 0.1168 | <0.001 | Significant increase |
| Clear | 0.1136 | <0.001 | Significant increase |

**Model Summary:**  
R² = 0.0266 | F = 170.43 (p < 0.001)

**Interpretation:**  
Rainy weather significantly reduces delivery success, while hot and clear conditions significantly improve success rates. Foggy weather has no statistically significant effect.

---

### (b) Delivery Delay Model

| Variable | Coefficient | P-value | Interpretation |
|----------|------------|--------|----------------|
| Intercept | 0.2275 | 0.000 | Base delay rate |
| Foggy | 0.0164 | 0.0325 | Slight increase |
| Rainy | 0.0722 | <0.001 | Strong increase |
| Hot | -0.0888 | <0.001 | Significant decrease |
| Clear | -0.0849 | <0.001 | Significant decrease |

**Model Summary:**  
R² = 0.0191 | F = 121.87 (p < 0.001)

**Interpretation:**  
Rainy weather significantly increases delays, while hot and clear conditions significantly reduce delays. Foggy weather has a mild but significant impact.

---

### (c) Delivery Failure Model

| Variable | Coefficient | P-value | Interpretation |
|----------|------------|--------|----------------|
| Intercept | 0.0604 | 0.000 | Base failure rate |
| Foggy | -0.0012 | 0.780 | Not significant |
| Rainy | 0.0134 | 0.0016 | Significant increase |
| Hot | -0.0280 | <0.001 | Significant decrease |
| Clear | -0.0287 | <0.001 | Significant decrease |

**Model Summary:**  
R² = 0.0048 | F = 30.18 (p < 0.001)

**Interpretation:**  
Rainy weather increases delivery failures, while hot and clear weather significantly reduce failure rates. Foggy weather has no meaningful effect.

---

## 💰 Weather Impact on Delivery Cost

| Metric | Value |
|--------|------|
| R² | 0.00005 |
| F-statistic | 0.257 |
| p-value | 0.937 |

**Interpretation:**  
Weather conditions do not significantly influence delivery cost. Cost remains driven by operational factors such as distance and package weight.

---

## 🛠️ Tools & Technologies

- Microsoft Excel  
- Regression Analysis  
- Statistical Techniques  

---

## 📁 Project Structure
---

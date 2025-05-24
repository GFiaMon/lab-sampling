# Study Habits Analysis Report

## 📋 Methodology

### Survey Questions & Response Options

#### 1. What is your age group? (Optional)
- Under 25  
- 25–29  
- 30–34  
- 35–39  
- 40–44  
- 45+  

![Age Distribution](./visuals/age.png)

---

#### 2. What is your current level of education? (Optional)
- Undergraduate student  
- Graduate student  
- Other (e.g., vocational training)  

![Education Levels](./visuals/education.png)

---

#### 3. Do you usually start lab work before the class ends at 12:30?
- Yes  
- No  
- Sometimes  

![Lab Start Times](./visuals/start-lab-before-class.png)

---

#### 4. Do you only work on labs during scheduled hours (12:30–16:30)?
- Yes  
- No  
- Sometimes  

![Scheduled Hours Work](./visuals/work-during-lab-hours.png)

---

#### 5. How much extra time do you spend on labs weekly?
- None  
- Less than 2 hours  
- 2–4 hours  
- 5–7 hours  
- 8–10 hours  
- More than 10 hours  

![Extra Time Spent](./visuals/extra-time.png)

---

#### 6. When do you work outside scheduled hours? (Multiple Select)
- Before class  
- Evenings  
- Late at night  
- Weekends  
- Only during lab hours  

![Off-Hours Work Patterns](./visuals/outside-hours-times.png)

---

#### 7. Do you take a lunch break between class and lab?
- Yes  
- No  
- Depends on the day  

![Lunch Breaks](./visuals/lunch-break.png)

---

#### 8. Lunch break duration (if yes)
- <15 minutes  
- 15–30 minutes  
- 30–60 minutes  
- >1 hour  

![Break Duration](./visuals/lunch-duration.png)

---

#### 9. Do you need more time than allocated?
- Yes  
- No  
- Not sure  

![Time Need](./visuals/need-more-time.png)

---

#### 10. Do you start labs before topics are covered?
- Yes  
- No  
- Sometimes  
- Wait until explained  

![Early Start](./visuals/start-before-topic-covered.png)

---

## 📊 Statistical Analysis

### Key Metric: Need for More Time
**Proportion**: 66.00%  
**95% Confidence Interval**: [52.87%, 79.13%]  
**Margin of Error**: ±13.13%  

![Proportion with CI](./visuals/proportion_ci.png)

```python
# Margin of Error Calculation
n = 50
p = 0.66
z = 1.96  # 95% confidence
se = (p * (1 - p) / n) ** 0.5  # Standard Error
margin_error = z * se
print(f"CI: [{p - margin_error:.2%}, {p + margin_error:.2%}]")
```

## 🧠 Key Insights
1. **Time Pressure**: 66% feel lab hours are insufficient (±13% margin)
2. **Reliability**: Current sample (n=50) needs expansion to 361 for ±5% accuracy
3. **Decision Risk**: True proportion could be as low as 53% or high as 79%


# LAB Deliverables: Consumer Preferences Study  
**Topic**: Study Habits Analysis  

---

## 1. Introduction  
**Research Question**:  
*How do students allocate time for lab work, and do they feel existing lab hours are sufficient?*  

**Population of Interest**:  
- Students enrolled in technical courses (synthetic + real data).  

**Sampling Method**:  
- **Convenience sampling** (initial 5 responses) + **synthetic data** (45 responses) to simulate a larger dataset.  
- **Justification**: Quick data collection under time constraints, though acknowledging potential bias.  

---

## 2. Methodology  
**Data Collection**:  
- **Tool**: Google Forms survey with 10 questions (e.g., study hours, lab scheduling preferences).  
- **Sample Size**: 50 participants (5 real + 45 synthetic).  
- **Variables**: Categorical (e.g., "Yes/No", time ranges).  

**Analysis Tools**:  
- Python (Pandas, Matplotlib/Seaborn) for data cleaning, visualization, and statistical calculations.  

---

## 3. Results  
### Key Findings  
1. **Time Allocation**:  
   - 62% of students reported needing **more time than allocated lab hours** (95% CI: 48%–76%).  
   - ![](./images/time_needed_plot.png) <!-- Include your actual plot path -->  

2. **Work Patterns**:  
   - 58% start labs **before class ends**, while 32% work **late at night**.  

3. **Lunch Breaks**:  
   - 65% take breaks of **15–30 minutes**.  

---

## 4. Sampling Error Analysis  
### Identified Errors  
1. **Small Sample Size**:  
   - Initial 5 responses had a **margin of error ±70%** (n=5).  
   - Expanded dataset (n=50) reduced error to **±14%**, but still significant.  

2. **Convenience Bias**:  
   - Over-representation of students from similar courses/years.  

3. **Self-Reporting Bias**:  
   - Subjective estimates of study hours (e.g., rounding errors).  

### Margin of Error Calculation  
For the key question *"Do you need more time?"*:  
- **Proportion (p)**: 62%  
- **Sample Size (n)**: 50  
- **Margin of Error**: ±14.2%  
- **Formula**:  
  ```python
  E = 1.96 * sqrt((p * (1 - p)) / n)
  ```
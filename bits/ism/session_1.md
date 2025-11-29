
# Introduction to Statistical Methods - Session 2 Notes
**Date:** November 1, 2025  
**Course:** S1-25_AIMLZC418  
**Instructor:** Prof. Pran Kumar  
**Duration:** 2h 3m 45s

---

## Table of Contents
1. [Session Overview](#session-overview)
2. [Recap from Previous Session](#recap-from-previous-session)
3. [Measures of Central Tendency](#measures-of-central-tendency)
4. [Properties of Arithmetic Mean](#properties-of-arithmetic-mean)
5. [Mode](#mode)
6. [Median](#median)
7. [Skewness](#skewness)
8. [Measures of Variability](#measures-of-variability)
9. [Standard Deviation and Variance](#standard-deviation-and-variance)
10. [Key Formulas](#key-formulas)

---

## Session Overview

This session covered:
- Arithmetic mean for frequency distributions
- Properties of arithmetic mean, median, and mode
- When to use each measure of central tendency
- Skewness in data distributions
- Measures of variability (range, standard deviation, variance)
- Practical applications and decision-making using statistical measures

---

## Recap from Previous Session

### Data Types
- **Quantitative Data:** Numerical data
- **Qualitative Data:** Categorical data (also called categorical data)

### Four Types of Measurement Scales
1. **Nominal Measurement:** Purely categorical (e.g., gender, religion)
2. **Ordinal Measurement:** Categorical with order
3. **Interval Measurement:** Numerical with meaningful differences
4. **Ratio Measurement:** Most powerful scale, includes all others

**Note:** Succeeding measurements are superior to preceding ones. Ratio scale is the most powerful.

### Purpose of Central Tendency
- Reduces large amounts of data to a single representative value
- Saves time in studying data
- Located in the middle part of the data
- Acts as a "leading value" or average
- Mathematically called "measure of central tendency"

### Three Main Measures
1. **Mean** - For quantitative data
2. **Median** - Positional measure
3. **Mode** - Most common value

---

## Measures of Central Tendency

### 1. Arithmetic Mean

#### Formula for Frequency Distribution
```
Ȳ = Σ(F × Y) / ΣF = Σ(F × Y) / N
```
Where:
- F = Frequency (or weight)
- Y = Variable value
- N = Total frequency (ΣF)

#### Example: TV Watching Hours
Data from 332 children in Bengaluru:
| Hours (Y) | Frequency (F) | F × Y |
|-----------|---------------|--------|
| 1         | 104           | 104    |
| 2         | 130           | 260    |
| 3         | 98            | 294    |
| **Total** | **332**       | **658**|

**Mean = 658 / 332 = 1.98 hours**

**Interpretation:** On average, each person spends 1.98 hours watching TV.

---

## Properties of Arithmetic Mean

### 1. **Stability/Consistency** ✅ (Positive Property)
- **Most stable measure** among all measures of central tendency
- Sample means cluster closely around population mean
- Difference typically within ±1 unit
- Advantage: Can estimate population mean from sample mean
- Works best with **homogeneous, uniform data**

**Example:**
- Large data set mean = 12.5
- Sample means: 12.41, 12.55, 12.58, 12.49
- All vary by less than ±1 from 12.5

### 2. **Affected by Extreme Values** ❌ (Negative Property)
- **Easily influenced by outliers**
- Outlier pulls mean toward extreme value
- Mean may not fall in middle of data
- Fails to be good representative

**Example:**
```
Data Set 1: 12, 13, 14, 1500  ← 1500 is outlier
Data Set 2: 12, 12.5, 13, 13.5  ← No outlier
```

**Solution when outliers exist:**
- Remove outlier (trim the data)
- Use **median** instead of mean
- **Median is not affected by outliers**

### 3. **Sum of Deviations = 0** ✅ (Positive Property)
**Formula:**
```
Σ(Y - Ȳ) = 0
```

**Example:**
```
Data: 10, 15, 20
Mean (Ȳ) = 15

Deviations:
10 - 15 = -5
15 - 15 = 0
20 - 15 = +5

Sum = -5 + 0 + 5 = 0 ✓
```

**This property is unique to arithmetic mean only.**

### 4. **May Not Be Actual Value** (Neutral Property)
- Mean is often a **theoretical value**
- Usually not equal to any actual data point
- Example: Mean = 39.6, but 39.6 may not exist in original data
- Not a problem - it's acceptable

### 5. **Easy to Compute** ✅ (Positive Property)
- Simple calculation
- No computational burden
- Software can easily calculate

---

## When to Use Arithmetic Mean

✅ **Use when:**
- Data is **quantitative** (numerical)
- No extreme values or outliers
- Data measured on **interval or ratio scale**
- Need **stability/consistency**
- Need to calculate: standard deviation, coefficient of variation, skewness
- Works for both **discrete and continuous** data

❌ **Don't use when:**
- Extreme values present
- Data is purely categorical
- Distribution is heavily skewed

---

## Mode

### Definition
**Mode** = The value that occurs **most frequently** in a data set
- Based on **maximum principle**
- Most popular measure in daily life
- No calculation needed - **observe directly**

### Real-Life Applications

#### 1. **Decision Making**
Example: Joining WILP course
- Asked 20 people for feedback
- 18 gave positive feedback ← **Maximum (Mode)**
- 2 gave negative feedback
- **Decision:** Join the course (based on mode)

#### 2. **Product Purchase**
- 16 people: negative feedback ← **Maximum (Mode)**
- 4 people: positive feedback
- **Decision:** Don't purchase (based on mode)

#### 3. **Business/Manufacturing**
- Manufacturer increases production for variety with **highest demand**
- Mode determines production levels

#### 4. **Politics**
- Entire politics based on mode
- Party with **majority votes** (maximum) wins
- Bill passes with **majority votes**
- Mode = majority principle

### Finding Mode

#### Example: Server Failures
```
Data: 1, 3, 0, 3, 3, 6, 3, 3, 2, 2, 4
```
- 3 appears **5 times** ← Maximum
- 2 appears 2 times
- Others appear 1 time each

**Mode = 3** (modal server failure)

### Types of Distributions
- **Unimodal:** One mode
- **Bimodal:** Two modes
- **Multimodal:** More than two modes
- **No mode:** All values occur once

### Properties of Mode

✅ **Positive Properties:**
1. Best for **qualitative/categorical data**
2. **First preference for nominal data**
3. Can apply to ordinal, interval, ratio data
4. **Not affected by extreme values**
5. No calculation needed - direct observation

❌ **Negative Property:**
1. **May not be unique** - can have multiple modes
2. **May not exist** - if all values occur once
3. **Ill-defined mode** creates confusion

### Empirical Relation for Mode
When mode is **bimodal/multimodal** or **doesn't exist**:

```
Mode = 3(Median) - 2(Mean)
```

**Note:** This is an **empirical relation** (based on observation of thousands of data sets), not mathematically derived.

---

## Median

### Definition
**Median** = Value at the **middle position** of ordered data
- **Positional measure**
- Divides data into two equal halves
- 50th percentile
- Middle value location

### Steps to Find Median
1. **Arrange data in order** (ascending or descending)
2. **Count observations (N)**
3. **Find middle position**
4. **Identify median value**

### Formula

#### For Odd Number of Observations
- Direct middle value
- **Actual median** can be found

#### For Even Number of Observations
- Two middle values exist
- **Median estimate** = (Y₁ + Y₂) / 2
- Take arithmetic mean of two middle values

### Cancellation Rule Method
1. Cancel smallest and largest values
2. Cancel second smallest and second largest
3. Continue until 1-2 values remain
4. If 1 value: that's the median
5. If 2 values: average them

### Example: Office Commute Time

**Arranged Data:** 29, 31, 35, 39, 39, 40, 43, 44, 44, 45

- N = 10 (even)
- Middle two values: 39 and 40
- **Median = (39 + 40) / 2 = 39.5 minutes**

**For same data:**
- Mean = 39.6
- Median = 39.5
- Mode = 39, 44 (bimodal) or 39.3 (using empirical formula)

**Observation:** Mean and median are **friendly/close to each other**

---

## Properties of Median

### 1. **Based on Middle 50%** ✅
- Uses only middle value(s)
- Not based on all observations
- Positional measure

### 2. **Not Affected by Extreme Values** ✅ (Most Important)
- **Safe measure** even with outliers present
- Extreme values at ends don't influence middle
- **Alternative to mean** when outliers exist

### 3. **Best for Ordinal Data** ✅
- **First preference:** Ordinal measurement scales
- Can also apply to interval and ratio data
- Sometimes used for nominal data

### 4. **Friendly to Mean** ✅
- Values usually close to each other
- Can replace mean when needed
- Support each other

---

## When to Use Median

✅ **Use when:**
- **Extreme values/outliers present** (most important)
- **Income data** (often has outliers)
- **Heavily skewed data**
- **Ordinal data**
- **Negotiating salary** (ask for median package, not mean)
- Want middle/typical value

❌ **Don't use when:**
- Need mathematical operations
- Want most stable measure
- Data is symmetric without outliers (use mean instead)

### Real-Life Application: Income Data

**Scenario:** Finding average income in an area
- Most people: low income (₹20,000 - ₹30,000)
- One person: very high income (₹50,00,000) ← Outlier

**If using Mean:**
- Inflated by high income
- Shows unrealistic average
- **Solution:** Remove outlier or use **median**

**If using Median:**
- Not affected by outlier
- Shows realistic middle income
- **Preferred measure**

---

## Skewness

### Definition
**Skewness** = Measure of asymmetry/imbalance in data distribution

### Types of Distributions

#### 1. **Symmetric Distribution** (Bell-Shaped/Normal)
```
Mean = Median = Mode
```
- **Best measure:** Arithmetic mean
- Data balanced on both sides
- Most values in center
- Example: Most students get middle marks

**Curve Shape:** Bell-shaped (symmetric)

---

#### 2. **Positively Skewed (Right Skew)**
```
Mode < Median < Mean
OR
Mean > Median > Mode
```
- **Tail extends to right** (higher values)
- Most students get **low marks**
- Few get high marks
- **Best measure:** Median or Mode
- **Outliers likely present**

**Curve Shape:** 
```
     Peak
    /  \___
   /       \___
  /            \___
```
Mode at peak, mean pulled right

---

#### 3. **Negatively Skewed (Left Skew)**
```
Mean < Median < Mode
```
- **Tail extends to left** (lower values)
- Most students get **high marks**
- Few get low marks
- **Best measure:** Median or Mode
- **Outliers likely present**

**Curve Shape:** 
```
        Peak
    ___/  \
___/       \
```
Mode at peak, mean pulled left

---

### Empirical Relationship (Revisited)
```
Mode = 3(Median) - 2(Mean)
```
- Valid for most skewed distributions
- Based on observation, not mathematical proof
- Holds true in 99% of cases

---

### Drawing Frequency Curves

**Using Histogram:**
1. Plot variable on x-axis
2. Plot frequency on y-axis
3. Draw rectangles (histogram)
4. Connect midpoints of rectangles
5. Curve passes through these points

**Examples:**

**Symmetric:**
```
  Frequency
     |
     |    _____
     |   /     \
     |  /       \
     | /         \
     |_____________
         Value
```

**Positive Skew:**
```
  Frequency
     |
     |___
     |   \___
     |       \___
     |___________\___
         Value
```

**Negative Skew:**
```
  Frequency
     |      ___
     |  ___/   
     |_/       
     |_____________
         Value
```

---

### Choosing Measure Based on Skewness

| Distribution Type | Best Measure | Reason |
|-------------------|--------------|---------|
| Symmetric | **Mean** | Most stable, mathematically sound |
| Positive Skew | **Median** or Mode | Not affected by outliers |
| Negative Skew | **Median** or Mode | Not affected by outliers |
| Multimodal | **Median** | Mode is confusing |

---

## Measures of Variability (Dispersion)

### Why Needed?
After finding mean/median/mode, we must verify:
- How well does the average represent the data?
- How close are values to the average?
- Is the average reliable?

### Key Concept
Even if two data sets have **same mean, median, and mode**, they may differ in **variability**.

**Example:**
```
Data Set 1: 3, 4, 5, 5, 5, 5, 5, 6, 7
Data Set 2: 1, 1, 2, 5, 5, 5, 8, 15, 15

Both have: Mean = 5, Median = 5, Mode = 5
```

**Which is better?** → Need to measure **variability**

---

### 1. Range

#### Definition
```
Range = Maximum Value - Minimum Value
```

#### Properties
- **Simplest measure**
- Shows **maximum distance** between any two values
- **Crude/imprecise measure**
- Uses only 2 observations
- **Not based on all observations**
- **Not reliable** for detailed analysis
- Good for **preliminary/first-hand** understanding

#### Example
```
Data: 2, 3, 5, 5, 5, 6, 7
Range = 7 - 2 = 5
```

---

### 2. Standard Deviation

#### Definition
**Standard Deviation (σ or s)** = Measure of **average/standard distance** of all observations from the mean

- Most important variability measure
- Shows if values are **clustered close** or **widely scattered**
- **Lower standard deviation** → Mean is better representative
- **Higher standard deviation** → Mean is poor representative

#### Key Insight
```
Low Standard Deviation:  ●●●|●●●  ← Values close to mean (|)
High Standard Deviation: ●  ●  |  ●  ●  ← Values far from mean (|)
```

---

### 3. Variance

#### Definition
**Variance (σ² or s²)** = Mean of squared deviations from mean
- **Theoretical measure**
- **Helping measure** for standard deviation
- Not directly interpretable
- Expressed in **squared units**

```
Standard Deviation = √Variance
```

---

## Standard Deviation and Variance

### Problem with Mean Deviation

**Mean Deviation Formula:**
```
Σ(X - μ) / N = 0 / N = 0
```
**Problem:** Always equals 0 (due to property of mean)
**Solution:** Use **squared deviations**

---

### Variance Formula

#### For Population (N ≥ 30)
```
σ² = Σ(X - μ)² / N
```

#### For Sample (N < 30)
```
s² = Σ(X - X̄)² / (N - 1)
```

**Where:**
- σ² = Population variance
- s² = Sample variance
- μ = Population mean
- X̄ = Sample mean
- N = Number of observations
- SS = Sum of squares = Σ(X - μ)²

---

### Standard Deviation Formula

#### For Population (N ≥ 30)
```
σ = √[Σ(X - μ)² / N]
```

#### For Sample (N < 30)
```
s = √[Σ(X - X̄)² / (N - 1)]
```

---

### Why N-1 for Small Samples?

#### Reason:
- Small samples naturally have **lower variance**
- Need to **adjust/correct** to approximate population variance
- Reducing denominator **increases** the variance value
- Makes sample variance closer to population variance

#### Mathematical Example:
```
Without correction: 3/4 = 0.75
With correction:    3/3 = 1.00  ← Larger value
```

#### When to Use:
- Use **N-1** when: N < 30 (small sample)
- Use **N** when: N ≥ 30 (large sample/population)

**Note:** This is based on **empirical study**, not theoretical proof.

---

### Units of Measurement

| Measure | Units | Practical Use |
|---------|-------|---------------|
| Data | kg, rupees, minutes | Original measurement |
| Variance | kg², rupees², minutes² | **Not practical** |
| Standard Deviation | kg, rupees, minutes | **Practical** ✓ |

**Standard Deviation is practical because:**
- Expressed in **original units**
- Can be interpreted directly
- Shows actual distance from mean

---

### Comparing Two Data Sets

#### Data Set 1
```
Values: 3, 4, 5, 5, 5, 5, 5, 6, 7
N = 9 (< 30, use N-1)
Mean = 5
Standard Deviation = 2.345
Range = 7 - 3 = 4 (Not shown as 8-2=6 in transcript)
```

#### Data Set 2
```
Values: 1, 1, 2, 5, 5, 5, 8, 15, 15
N = 9 (< 30, use N-1)
Mean = 5
Standard Deviation = 4.093
Range = 15 - 1 = 14
```

#### Analysis
| Measure | Data Set 1 | Data Set 2 |
|---------|------------|------------|
| Mean | 5 | 5 |
| Std Dev | 2.345 | 4.093 |
| Range | 6 | 14 |
| Variability | **Low** ✓ | **High** |
| Decision | **Select** | Discard |

**Conclusion:** Data Set 1 is better because:
- Lower standard deviation
- Values clustered closer to mean
- Mean is better representative

---

### Interpretation of Standard Deviation

**Example:** Standard Deviation = 2.345

**Meaning:** 
- On average, observations are **2.345 units away** from the mean
- Shows degree of **spreadness/clusterness**
- Lower value = more reliable mean
- Higher value = less reliable mean

---

## Key Formulas

### Measures of Central Tendency

#### Arithmetic Mean
```
Simple: Ȳ = ΣY / N

Frequency: Ȳ = Σ(F × Y) / ΣF

Weighted: Ȳ = Σ(W × Y) / ΣW
```

#### Median
```
Odd N: Middle value directly

Even N: Median = (Y₁ + Y₂) / 2
```

#### Mode
```
Direct: Most frequent value

Empirical: Mode = 3(Median) - 2(Mean)
```

### Measures of Variability

#### Range
```
Range = Maximum - Minimum
```

#### Variance
```
Population: σ² = Σ(X - μ)² / N

Sample: s² = SS / (N - 1) = Σ(X - X̄)² / (N - 1)
```

#### Standard Deviation
```
Population: σ = √[Σ(X - μ)² / N]

Sample: s = √[Σ(X - X̄)² / (N - 1)]
```

### Relationships

#### Sum of Deviations
```
Σ(X - X̄) = 0  (Always, for mean only)
```

#### Skewness
```
Symmetric: Mean = Median = Mode

Positive Skew: Mean > Median > Mode

Negative Skew: Mean < Median < Mode

Empirical: Mode = 3(Median) - 2(Mean)
```

---

## Summary Tables

### When to Use Each Measure

| Measure | Data Type | Best For | Affected by Outliers? |
|---------|-----------|----------|----------------------|
| **Mean** | Quantitative | Symmetric data, Ratio/Interval scales | ✗ Yes |
| **Median** | Quantitative/Ordinal | Skewed data, Ordinal scales, Income data | ✓ No |
| **Mode** | Qualitative/Quantitative | Nominal data, Decision making | ✓ No |

---

### Properties Comparison

| Property | Mean | Median | Mode |
|----------|------|--------|------|
| Stability | High ✓ | Medium | Low |
| Affected by outliers | Yes ✗ | No ✓ | No ✓ |
| Mathematical properties | Strong ✓ | Weak | Weak |
| Uniqueness | Always unique ✓ | Always unique ✓ | May not be unique ✗ |
| Calculation | Easy | Easy | Very easy |
| Uses all observations | Yes | No | No |

---

### Practical Applications

| Situation | Recommended Measure | Reason |
|-----------|-------------------|---------|
| Student exam scores (normally distributed) | Mean | Symmetric, no outliers |
| Income in area with billionaires | Median | Outliers present |
| Most popular product | Mode | Maximum principle |
| Salary negotiation | Median | Represents middle, not extreme |
| Quality control (normally distributed) | Mean | Need mathematical properties |
| Customer satisfaction ratings | Mode or Median | Ordinal data |
| Server failures | Mode | Most common occurrence |

---

## Important Concepts

### 1. Outliers
**Definition:** A value that is:
- Located at **extreme right** OR **extreme left**
- AND occurs **only one time**

**Impact:**
- Affects mean significantly
- Does not affect median or mode
- Should be removed or use median

---

### 2. Stability/Consistency
**What it means:**
- Sample means cluster close to population mean
- Variation between sample means is minimal (±1 typically)
- Can estimate population parameter from sample

**Which measure:**
- **Mean** has highest stability
- **Median** has medium stability
- **Mode** has lowest stability

---

### 3. Software vs Manual Calculation
**Modern Approach:**
- Calculations done by software (Excel, SPSS, SAS, R, Python)
- Focus on **interpretation**, not calculation
- Understand **properties and behavior**
- Know **when to apply** each measure

---

## Practice Questions & Answers

### Question 1
**A sample of four scores has a sum of squares (SS) = 24. What is the variance?**

**Solution:**
```
N = 4 (< 30, use N-1)
SS = 24

Variance = SS / (N-1)
         = 24 / (4-1)
         = 24 / 3
         = 8

Answer: 8
```

---

### Question 2
**A sample systematically has less variability than a population. True or False?**

**Answer: True**

**Reason:**
- Sample size is smaller than population
- Naturally has less variation
- That's why we use N-1 correction for samples

---

### Question 3
**The standard deviation is the distance from the mean to the farthest point on the distribution curve. True or False?**

**Answer: False**

**Reason:**
- Standard deviation uses **ALL observations**, not just farthest
- Formula: √[Σ(X - X̄)² / N] includes all values
- **Range** uses farthest points, not standard deviation

---

## Next Session Preview

### Topics to be Covered:
1. **Box and Whisker Plot**
   - Most important graphical tool
   - Identifying outliers in large data sets
   - Quartile deviation
2. **Probability Concepts**
   - Foundation for inferential statistics

---

## Key Takeaways

1. ✅ **Mean** is most stable but affected by outliers
2. ✅ **Median** is best for skewed data and when outliers present
3. ✅ **Mode** is best for categorical data and decision making
4. ✅ Use **standard deviation** to check reliability of mean
5. ✅ Lower variability = better representative average
6. ✅ For samples (N < 30), use N-1 in denominator
7. ✅ Understand **when to use** each measure, not just how to calculate

---

## Statistical Concepts Hierarchy

```
Data Analysis
    |
    ├── Descriptive Statistics (Past patterns)
    |       |
    |       ├── Central Tendency (Single value)
    |       |       ├── Mean (Quantitative, symmetric)
    |       |       ├── Median (Ordinal, skewed)
    |       |       └── Mode (Categorical, maximum)
    |       |
    |       └── Variability (Spread/reliability)
    |               ├── Range (Simple, 2 points)
    |               ├── Variance (Theoretical, squared)
    |               └── Standard Deviation (Practical, original units)
    |
    └── Inferential Statistics (Future predictions)
            ├── Population → Large data
            └── Sample → Small data
```

---

## Important Notes

### Remember:
1. **Arithmetic mean** uses all observations (Σ mechanism)
2. **Median** uses only middle 1-2 observations
3. **Mode** uses most frequent value
4. **Σ(X - X̄) = 0** is unique to mean only
5. **Empirical relations** are observation-based, not mathematically proven
6. **N-1 correction** applies only when N < 30
7. **Standard deviation** is always in **original units**

### Empirical Relations:
```
Mode = 3(Median) - 2(Mean)  [When mode is ill-defined]
```

### Distribution Types:
```
Symmetric:  Mean = Median = Mode
Right Skew: Mean > Median > Mode
Left Skew:  Mean < Median < Mode
```

---

## Additional Resources

- **PPT:** Available on Microsoft Teams (not Takshila)
- **Recorded Session:** Automatically uploaded to MS Teams
- **Software Tools:** Excel, SPSS, SAS, R, Python for calculations
- **Next Session:** Box plots, Quartiles, Probability

---

## Glossary

| Term | Definition |
|------|------------|
| **Central Tendency** | Single value representing entire data set |
| **Variability** | Measure of spread/dispersion in data |
| **Outlier** | Extreme value occurring once at data ends |
| **Skewness** | Measure of asymmetry in distribution |
| **Deviation** | Distance of observation from mean |
| **Variance** | Mean of squared deviations (theoretical) |
| **Standard Deviation** | Square root of variance (practical) |
| **Population** | Large/complete data set (N ≥ 30) |
| **Sample** | Small subset of data (N < 30) |
| **SS (Sum of Squares)** | Σ(X - X̄)² |
| **Empirical** | Based on observation, not mathematical proof |
| **Unimodal** | Distribution with one mode |
| **Bimodal** | Distribution with two modes |
| **Multimodal** | Distribution with more than two modes |
| **Symmetric** | Balanced distribution (bell-shaped) |
| **Normal Distribution** | Bell-shaped, Mean = Median = Mode |

---

**End of Session 2 Notes**

*"Focus on understanding when to apply statistical measures, not just how to calculate them. Software handles calculations; we need to interpret and make decisions."* - Prof. Pran Kumar

# 🚴‍♂️ VoltBike Innovations: E-Bike Data Analytics Project

> **A comprehensive data analysis project for the Python Data Associate certification**

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

## 📋 Project Overview

This project involves a detailed data analysis for **VoltBike Innovations**, a leading manufacturer of high-performance electric bicycles (e-bikes). As a member of the data analysis team, the goal is to provide actionable insights to address production cost management and customer satisfaction challenges.

### Company Background
VoltBike Innovations specializes in designing and manufacturing cutting-edge e-bikes with advanced features including:
- ⚡ Varying motor power outputs
- 🔋 Advanced battery technologies
- 🏎️ High-performance specifications
- 🌍 Urban mobility solutions

## 📊 Dataset Overview

The analysis is based on **500 e-bike records** contained in `ebike_data.csv`, featuring the following attributes:

### Data Features

| Feature | Type | Description | Range/Categories |
|---------|------|-------------|-------------------|
| **bike_type** | Categorical | Type of e-bike | `standard`, `folding`, `mountain`, `road` |
| **frame_material** | Categorical | Frame construction material | `aluminum`, `steel`, `carbon fiber` |
| **production_cost** | Numerical | Manufacturing cost in USD | Continuous |
| **assembly_time** | Numerical | Assembly duration in minutes | Continuous |
| **top_speed** | Numerical | Maximum velocity in km/h | Continuous |
| **battery_type** | Categorical | Battery chemistry | `li-ion`, `nimh`, `lead acid` |
| **motor_power** | Numerical | Motor output in watts | Continuous |
| **customer_score** | Numerical | Satisfaction rating (1-10 scale) | 1.0 - 10.0 |

## 🎯 Project Tasks

### Task 1: Data Cleaning & Validation ✅

**Objective:** Ensure data quality by addressing missing values and inconsistencies.

**Approach:**
- ✓ Standardized categorical values (fixed inconsistent casing like 'STEel' → 'steel')
- ✓ Implemented strategic missing value imputation:
  - **bike_type**: Missing values replaced with `'standard'` (most common)
  - **frame_material**: Missing values replaced with `'unknown'` category
  - **production_cost & motor_power**: Imputed with median (resistant to outliers)
  - **assembly_time, top_speed & customer_score**: Imputed with mean (central tendency)
  - **battery_type**: Standardized missing markers (`'-'`) to `'other'` category

**Output:** Clean, validated dataframe ready for analysis

---

### Task 2: Comparative Analysis by Bike Type 📈

**Objective:** Understand how different e-bike models impact key business metrics.

**Key Metrics Analyzed:**
- Average production cost per bike type
- Average assembly time per bike type
- Average customer satisfaction scores per bike type

**Expected Insights:**
- Identify which bike types are most cost-efficient
- Determine assembly complexity variations
- Reveal customer satisfaction patterns by bike category
- Support product portfolio optimization decisions

**Output:** Consolidated comparison table with 4 bike categories

---

### Task 3: Correlation & Statistical Analysis 📉

**Objective:** Investigate the relationship between production costs and customer satisfaction.

**Statistical Measures Calculated:**

| Metric | Purpose |
|--------|---------|
| **Production Cost Mean & SD** | Understand cost distribution and variability |
| **Customer Score Mean & SD** | Assess satisfaction baseline and consistency |
| **Pearson Correlation Coefficient** | Quantify strength and direction of cost-satisfaction relationship |

**Key Finding:** Analyzing whether higher production costs correlate with improved customer satisfaction or if cost optimization is possible without sacrificing quality.

**Output:** Comprehensive statistical summary for strategic decision-making

---

## 🔍 Key Analysis Insights

The project enables stakeholders to answer critical business questions:

1. **Cost Management**: Which bike types have the highest/lowest production costs?
2. **Quality vs. Cost Trade-off**: Is there a positive correlation between production investment and customer satisfaction?
3. **Assembly Efficiency**: Which designs are quickest to manufacture?
4. **Product Strategy**: Where should resources be allocated for maximum ROI?

## 📁 Project Structure

```
📦 Python-Data-Associate-Exam
├── 📄 README.md                 # Project documentation (this file)
├── 📊 ebike_data.csv            # Raw dataset (500 e-bike records)
├── 📓 notebook.ipynb            # Analysis notebook with tasks 1-3
└── 📈 Analysis outputs          # Cleaned data & statistical summaries
```

## 🛠️ Technical Stack

- **Language:** Python 3.x
- **Libraries:**
  - `pandas` - Data manipulation and analysis
  - `numpy` - Numerical computations (via pandas)
  - `scipy.stats` - Statistical analysis

## 💡 Use Cases & Applications

✅ **Production Optimization** - Identify cost-saving opportunities  
✅ **Quality Assurance** - Maintain customer satisfaction standards  
✅ **Portfolio Management** - Strategic decisions on product lines  
✅ **Supply Chain** - Assembly time insights for capacity planning  
✅ **Market Analysis** - Customer satisfaction trends across segments  

## 🎓 Learning Outcomes

This project demonstrates proficiency in:
- **Data Cleaning**: Handling missing values and data inconsistencies
- **Data Aggregation**: Grouping and summarizing data by categories
- **Statistical Analysis**: Computing correlation and distribution metrics
- **Business Analytics**: Translating data into actionable insights
- **Python Proficiency**: Using pandas for real-world data scenarios

## 📝 Notes for Analysts

- All numerical calculations are rounded to 2 decimal places for consistency
- Missing data imputation follows domain knowledge best practices
- Analysis assumes data accuracy post-cleaning phase
- Results should be validated against domain experts before implementation

---

**Project Type:** Python Data Associate Certification Exam  
**Difficulty Level:** Intermediate  
**Duration:** Multi-part analysis project  
**Last Updated:** 2024

---

*For questions or clarifications about this analysis, please refer to the analysis notebook (`notebook.ipynb`) which contains detailed code implementations for all tasks.*

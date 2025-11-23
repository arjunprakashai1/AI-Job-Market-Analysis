# AI Job Market: Exploratory Data Analysis

[![Python](https://img.shields.io/badge/Python-3.11-blue.svg)](https://www.python.org/)
[![Status](https://img.shields.io/badge/Status-Active-success.svg)]()

## 📋 Table of Contents
- [Overview](#overview)
- [Research Questions](#research-questions)
- [Dataset](#data)
- [Installation](#installation)
- [Analysis & Findings](#analysis--findings)
- [Technologies Used](#technologies-used)
- [Conclusion]()



## 🎯 Overview

The AI job market is rapidly evolving, making it difficult for job seekers and industry leaders to understand the current landscape. This analysis seeks to answer critical questions such as: **What are the most financially rewarding skills?** and **How does compensation vary by experience level and location?**

The primary objective of this project is to conduct a comprehensive **Exploratory Data Analysis (EDA)** on the global Artificial Intelligence job market to extract actionable insights that can guide:
- **Job seekers** in identifying high-demand skills and lucrative career paths
- **Employers** in understanding competitive compensation trends
- **Industry analysts** in tracking market evolution and emerging patterns

## ❓ Research Questions

This analysis investigates six key questions about the AI job market:

1. **Which industry has the most job openings?**
2. **How does the median salary vary for different jobs?**
3. **Which are the top-paying and most in-demand skills?**
4. **Do experience level and company size affect salary?**
5. **What are the most preferred tools by companies?**
6. **How have job postings trended over the months?**

## 📊 Data

### Data Source
The dataset used in this analysis is sourced from Kaggle. This synthetic data represents AI-related job postings from sep 2023 to sep 2025 across.

### Dataset Description
- **Size**: 2000 job postings
- **Time Period**: Sep 2023 to Sep 2025
- **Last Updated**: Nov 2025

### Key Features
The dataset includes the following attributes:

| Feature | Description | Data Type |
|---------|-------------|-----------|
|`job_id` | Unique Id | Int |
| `company_name` | Hiring company | String |
| `industry` | Industry sector | Categorical |
| `job_title` | Job position title | String |
|`skills_required` | Required skills | List |
| `experience_level` | Required experience (Entry/Mid/Senior) | Categorical |
|`employment_type` | (Full-time, Contract, Remote, Internship) | Categorical |
| `location` | Job location (city/country) | String |
| `median_salary` | Job salary | Int |
| `posted_date` | Date job was posted | DateTime |
| `company_size` | Organization size (Startup/Mid/Large) | Categorical |
| `tools_preferred` | Preferred tools/technologies | List |


### Data Preprocessing
- Converted date fields to datetime format
- Converted skill fields and tools from string to list
- Removed duplicate job postings
- Filtered outliers in salary data

### Data Limitations

#### 1. No Real-World Validity

Data does not represent actual job market conditions
Findings cannot be used for real business decisions or career planning
Patterns observed are artifacts of the generation process, not market realities


#### 2. Simplified Relationships

Correlations between variables (e.g., skills and salary) are predetermined by generation logic
Real-world complexities, irregularities, and exceptions are not captured
Missing nuanced interactions between multiple factors


#### 3. Lack of Market Dynamics

Does not reflect actual supply-demand economics
Temporal trends are simulated and may not match real seasonal patterns
Cannot capture sudden market shifts, economic events, or industry disruptions


#### 4. Artificial Distributions

Statistical distributions may not match real-world data patterns
Outliers and edge cases may be under-represented or over-simplified
Variance in data may be artificially constrained


#### 5. No Geographic Accuracy

Location-based salary differences are estimated, not based on actual cost of living
Regional industry concentrations may not reflect reality
Cultural and regulatory factors affecting employment are not modeled


#### 6. Skills and Tools Bias

Skill combinations may not reflect actual job requirements
Tool preferences are based on assumptions, not employer data
Emerging technologies and skills may be missing


#### 7. Temporal Validity

Data does not capture current market conditions
Cannot be used to predict future trends
No reflection of recent industry events or technological shifts


#### 8. Sampling Bias

May over-represent or under-represent certain job types, industries, or experience levels
Distribution across categories may not match real market proportions
Missing representation of niche roles or emerging positions

## 🚀 Installation

### Prerequisites
- Python 3.8 or higher
- conda package manager

### Setup Instructions

1. **Create a conda environment**
```bash
conda create -n ai-job-market python=3.11
conda activate ai-job-market
```

2. **Install required packages** 
```bash
conda install -c conda-forge pandas numpy matplotlib seaborn  jupyter 
```

3. **Alternative: Using pip with conda environment**
```bash
pip install -r requirements.txt
```

### Required Dependencies
```
pandas>=1.5.0
numpy>=1.23.0
matplotlib>=3.6.0
seaborn>=0.12.0
jupyter>=1.0.0
```


## 📈 Analysis & Findings

### Key Insights

**Industry Distribution**


**Salary Analysis**
- [Key findings about median salaries across different roles]

**In-Demand Skills**
- [Top skills and their correlation with compensation]

**Experience & Company Size Impact**
- [How these factors influence salary ranges]

**Tool Preferences**
- [Most commonly required tools and technologies]

**Temporal Trends**
- [Job posting patterns over time]

For detailed findings, see the [full analysis report](results/reports/analysis_summary.md).

## 🛠️ Technologies Used

- **Python 3.11** - Core programming language
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computations
- **Matplotlib & Seaborn** - Static visualizations
- **Jupyter Notebook** - Interactive development environment


## 🎯 Conclusion


---

**Note**: This is an educational/research project. The findings should be interpreted within the context of the data limitations and methodology described above.

*Last Updated: [Date]*
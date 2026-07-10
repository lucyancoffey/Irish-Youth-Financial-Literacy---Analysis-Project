# Financial Literacy Among Young Irish Adults (18–29)

## End-to-End Excel Dashboard & Python Analysis

![Dashboard Preview](/Images/dashboard.png)

# Overview

Financial literacy has become increasingly important as young adults face rising living costs, higher levels of debt, and more complex financial decisions than previous generations. Understanding how financially prepared young people are is essential for developing effective education initiatives and improving long-term financial wellbeing.

This project investigates the financial literacy of **young Irish adults aged 18–29** using data from the OECD/[INFE 2023 International Survey of Adult Financial Literacy](https://www.oecd.org/en/publications/oecd-infe-2023-international-survey-of-adult-financial-literacy_56003a32-en/support-materials.html).

The objective was to build an **end-to-end data analytics project** that demonstrates practical analyst skills by taking a real-world dataset through the complete analytics workflow:

- Cleaning and transforming raw survey data in **Microsoft Excel**
- Designing an interactive dashboard
- Performing exploratory data analysis in **Python**
- Producing publication-quality visualisations
- Communicating meaningful insights through data storytelling

While Excel serves as the primary analytical tool throughout this project, Python is used as a companion environment to validate findings, explore additional trends, and create supporting visualisations.

Ultimately, this project forms part of my wider research into developing digital tools and educational resources that help improve financial literacy among young people in Ireland.

# Project Workflow

```
OECD/INFE 2023 Survey Data
            │
            ▼
     Excel Data Cleaning
            │
            ▼
 Excel Dashboard
            │
            ▼
 Python Companion Analysis
            │
            ▼
   Insights & Recommendations
```

# Research Questions

This project was designed to answer four key questions:

1. What is the overall financial literacy level of Irish adults aged 18–29?
2. How do Ireland's financial knowledge, behaviour and attitudes compare with OECD averages?
3. Which financial knowledge topics present the greatest challenges for young Irish adults?
4. What insights can help improve financial education and awareness among young people?

# Data Source

**Dataset**

OECD/INFE 2023 International Survey of Adult Financial Literacy

The survey measures financial literacy across **39 countries**, evaluating participants using three key dimensions:

- Financial Knowledge
- Financial Behaviour
- Financial Attitudes

These three components combine to produce an overall Financial Literacy Score.

For this project, I focused specifically on the **18–29 age group**, allowing Ireland's young adults to be benchmarked against both OECD averages and international peers.

# Technologies Used

| Technology | Purpose |
|------------|---------|
| Microsoft Excel | Data cleaning, transformation, dashboard creation |
| Python | Exploratory data analysis |
| Pandas | Data manipulation |
| Matplotlib | Data visualisation |
| Seaborn | Statistical graphics |
| Jupyter Notebook | Python analysis companion |
| Visual Studio Code | Development environment |
| Git & GitHub | Version control and project publishing |

# Skills Demonstrated

- Excel Dashboard Development
- Data Cleaning & Preparation
- Exploratory Data Analysis (EDA)
- Comparative Statistical Analysis
- Data Visualisation
- Data Storytelling
- Research Communication
- Git Version Control

# Project Structure

```
Irish_Youth_Financial_Literacy/

│

├── Dashboard/
│   └── Irish_Financial_Literacy_Project.xlsx
│
├── Images/
│   ├── chart1_ireland_profile.png
│   ├── chart2_global_ranking.png
│   ├── chart3_knowledge_questions.png
|   ├── dashboard.png
│   └── chart4_youth_penalty.png
|
├── Python_Analysis/
│   └── Young_Irish_Financial_Literacy_Analysis.ipynb
│
└── README.md
```

# Data Preparation

The original OECD workbook contained multiple worksheets covering different countries, age groups and financial literacy indicators.

Before analysis, the dataset was prepared in Excel by:

- Cleaning inconsistent entries
- Standardising variable names
- Filtering respondents aged **18–29**
- Creating calculated metrics
- Preparing lookup tables
- Building dashboard-ready datasets
- Exporting analysis-ready tables for Python

Using Excel as the primary cleaning tool ensured consistency between the dashboard and the Python notebook.

# Dashboard

The dashboard was designed to provide an interactive overview of financial literacy among young Irish adults.

### Dashboard Features

- KPI summary cards
- Financial Literacy Score
- Financial Knowledge Score
- Financial Behaviour Score
- Financial Attitude Score
- OECD benchmark comparisons
- International country rankings
- Interactive filtering
- Clean, publication-style design

### Dashboard Preview

![Dashboard](/Images/dashboard.png)

# Python Companion Analysis

While Excel was used to build the dashboard, Python served as a companion analysis environment that allowed deeper exploration of the cleaned dataset.

The notebook includes:

- Exploratory Data Analysis
- Country benchmarking
- Comparative visualisations
- Financial knowledge analysis
- Youth Penalty analysis
- Publication-quality charts
- Supporting insights

Notebook:

[Young Irish Financial Literacy Analysis](/Python_Analysis/Young_Irish_Financial_Literacy_Analysis.ipynb)

# Analysis & Findings

## 1. Ireland's Financial Literacy Profile

To understand Ireland's performance, I compared the country's financial knowledge, behaviour and attitudes against the OECD average for the same age group.

### Visualisation

```python
fig, ax = plt.subplots(figsize=(10, 6))

for bar in bars_ire:
    ax.text(bar.get_x() + bar.get_width()/2,
        bar.get_height() + 0.8,
        f'{bar.get_height():.2f}',
        ha='center', va='bottom', fontsize=10, fontweight='bold', color=TEAL)

for bar in bars_oecd:
    ax.text(bar.get_x() + bar.get_width()/2,
        bar.get_height() + 0.8,
        f'{bar.get_height():.2f}',
        ha='center', va='bottom', fontsize=10, fontweight='bold', color=DARK)

plt.show()
```

### Results

![Ireland Profile](/Images/chart1_ireland_profile.png)

### Insights

- Ireland scores above the OECD average across every financial literacy dimension.
- Financial Behaviour is Ireland's strongest area, ranking among the highest internationally.
- Financial Attitudes remain noticeably weaker than Behaviour, suggesting strong day-to-day money management but weaker long-term financial planning.
- The gap between Behaviour and Attitudes indicates opportunities for improved financial education around future planning.

## 2. International Ranking

To benchmark Ireland internationally, I compared overall financial literacy scores across all participating countries.

### Results

![Global Ranking](/Images/chart2_global_ranking.png)

### Insights

- Ireland ranks **3rd out of 39 countries** overall for financial literacy among young adults.
- Ireland comfortably exceeds the OECD benchmark.
- OECD member countries generally outperform non-OECD countries, although there are notable exceptions.

## 3. Financial Knowledge Questions

To identify specific areas for improvement, I analysed performance across the individual financial knowledge questions.

### Results

![Knowledge Questions](/Images/chart3_knowledge_questions.png)

### Insights

- Compound interest remains one of the weakest performing concepts.
- Inflation and risk diversification also show room for improvement.
- Basic financial numeracy performs comparatively well.
- These findings highlight where future financial education initiatives could have the greatest impact.

## 4. Youth Penalty Analysis

The final analysis compared financial literacy scores between the **18–29** and **30–59** age groups.

This "Youth Penalty" measures how much younger adults underperform older adults within each country.

### Results

![Youth Penalty](/Images/chart4_youth_penalty.png)

### Insights

- Most countries experience a negative Youth Penalty, indicating lower financial literacy among younger adults.
- Ireland performs relatively well compared with many international peers.
- Nevertheless, younger adults still score below the middle-aged population, reinforcing the need for earlier financial education.

# Key Findings

This analysis produced several important findings:

- Ireland ranks **3rd out of 39 countries** for overall financial literacy among young adults.
- Financial Behaviour is Ireland's strongest performing dimension.
- Financial Attitudes lag behind Behaviour, highlighting weaker long-term financial planning.
- Knowledge surrounding compound interest and inflation remains relatively weak.
- Ireland performs strongly internationally but still exhibits a measurable Youth Penalty compared with older adults.

# Recommendations

Based on these findings, several opportunities exist to improve financial literacy among young Irish adults:

- Introduce practical financial education earlier in secondary schools and universities.
- Increase awareness of compound interest and long-term investing.
- Promote budgeting and financial planning tools designed specifically for young adults.
- Continue benchmarking Ireland against OECD countries to monitor future progress.
- Develop digital tools that make financial education more engaging and accessible.

# What I Learned

This project significantly strengthened both my technical and analytical skills.

In particular, I developed experience in:

- Cleaning and transforming real-world datasets using Excel.
- Designing interactive dashboards that communicate insights effectively.
- Using Python to validate findings and create publication-quality visualisations.
- Combining Excel and Python into a single analytics workflow.
- Presenting analytical findings through clear, evidence-based storytelling.

Most importantly, this project reinforced the importance of selecting the right tool for each stage of the analytics process rather than relying on a single technology.

# Challenges

Some of the key challenges included:

- Preparing a large multi-sheet OECD dataset for analysis.
- Designing a dashboard that balanced detail with usability.
- Selecting visualisations that clearly communicated international comparisons.
- Interpreting behavioural trends without overstating conclusions.
- Maintaining consistency between Excel outputs and Python analysis.

# Future Improvements

There are several opportunities to extend this project further:

- Develop an interactive Power BI dashboard.
- Perform statistical significance testing.
- Build predictive models using demographic variables.
- Compare results with future OECD financial literacy surveys.

# Conclusion

This project demonstrates a complete end-to-end analytics workflow using real-world financial literacy data.

Beginning with raw OECD survey data, I cleaned and transformed the dataset in Excel, designed an interactive dashboard, and complemented the analysis with Python-based exploratory data analysis and visualisation.

Beyond demonstrating technical skills in Excel and Python, this project showcases my ability to communicate insights, interpret complex datasets, and present evidence-based recommendations that could contribute to improving financial education among young adults in Ireland.

As I continue developing tools and resources to support financial wellbeing, this analysis provides a strong foundation for future research into financial behaviour, education and decision-making.
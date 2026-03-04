![GitHub Repo Size](https://img.shields.io/github/repo-size/ssaagastume11/oscars-demographics-analysis)
![Last Commit](https://img.shields.io/github/last-commit/ssaagastume11/oscars-demographics-analysis)

# 🏆 Oscars Demographics Analysis (1928–Present)

This project analyzes demographic trends among Academy Award winners across major categories including Best Actor, Best Actress, Best Supporting Actor, Best Supporting Actress, and Best Director.  

The analysis explores long-term representation patterns related to gender, race/ethnicity, age, religion, and sexual orientation to better understand how diversity among winners has evolved since 1928.

---

## 📦 Dataset

**Source**: Demographics of Academy Awards (Oscars) Winners  
**Platform**: Kaggle (public dataset)  
**Coverage**: 1928 – Present  

**Location**: Stored in the `data/` folder  
**Filename**: `Oscars-demographics-DFE.csv`

**Key Fields Include**:
- Person (Winner Name)
- Award Category
- Year of Award
- Movie
- Date of Birth
- Age at Award (calculated)
- Race / Ethnicity
- Religion
- Sexual Orientation
- Birthplace
- Gender Category

---

## 🔍 Business Task

The objective of this analysis is to examine representation trends among Oscar winners by:

- Identifying demographic patterns over decades
- Measuring changes in gender and racial representation
- Analyzing age trends at the time of award
- Comparing diversity patterns across award categories
- Evaluating long-term progress in industry inclusion

---

## 📊 Tools & Technology

- **Google BigQuery** – Data cleaning, transformation, and aggregation
- **SQL** – Structured analysis queries
- **Tableau Public** – Interactive dashboard visualization
- **Google Slides** – Stakeholder-ready presentation
- **Git & GitHub** – Version control and project sharing

---

## 📁 Project Structure

```plaintext
oscars-demographics-analysis/
├── data/
│   └── Oscars-demographics-DFE.csv
├── sql/
│   ├── Step_1_Ask.sql
│   ├── Step_2_Prepare.sql
│   ├── Step_3_Process.sql
│   ├── Step_4_Analyze.sql
│   └── Step_6_Act.sql
├── visuals/
│   ├── winners_by_decade.png
│   ├── gender_trends.png
│   └── avg_age_by_category.png
├── tableau/
│   └── Oscars_Dashboard_Link.md
├── presentation/
│   └── Oscars_Demographics_Presentation.md
└── README.md
```

---

## 🧮 Sample SQL Query (Gaming Hours vs Performance)

```SQL
SELECT
  award,
  award_decade,
  gender_category,
  COUNT(*) AS total_winners,
  AVG(age_at_award) AS avg_age_at_award
FROM
  `plenary-ability-463920-b3.oscars_analysis.demographic_trends_by_decade`
GROUP BY
  award,
  award_decade,
  gender_category
ORDER BY
  award_decade;
```

---

## 📈 Analysis Output

Key visual outputs stored in the visuals/ folder include:

- 📊 Winners by Decade
- 👥 Gender Representation Trends
- 🌍 Race/Ethnicity Distribution by Category
- 🎂 Average Age at Award by Category
- 🎬 Category-Based Representation Comparisons

---

## 📊 Interactive Tableau Dashboard

Explore the interactive dashboard analyzing demographic representation among Oscar winners:

🔗 **Tableau Public Dashboard:**  
[Oscars Demographics Analysis Dashboard](https://public.tableau.com/views/OscarsDemographicsAnalysis/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

This dashboard allows users to interactively explore:

- Representation trends by decade
- Gender distribution across award categories
- Race/ethnicity patterns over time
- Average age at award
- Category-based diversity comparisons

---

## 🧾 Presentation

The final presentation (located in the presentation/ folder) covers:

- Project objective and research questions
- Data preparation and cleaning steps
- Processing and aggregation logic
- Key demographic insights
- Actionable recommendations

---

## 🔎 Key Findings
- Represenation patterns have evolved gradually over decades.
- Gender distribution varies significantly by award category.
- Certain decades show noticeable shifts in demographics trends.
- Age at award differs across acting and directing categories.

---

## 📌 Recommendations

- Continue monitoring long-term demographic trends
- Increase transparency in representation reporting
- Support inclusive talent development pipelines
- Use data-driven metrics to track industry diversity progress

---

## 🙌 Acknowledgments
- Dataset courtesy of [Felix Mejia on Kaggle](https://www.kaggle.com/datasets/fmejia21/demographics-of-academy-awards-oscars-winners)
- Analysis conducted using Google Cloud BigQuery, SQL, Tableau and Google Slides.

---

👨‍💻 Author

**Sergio E. Sagastume**
Data Analyst | SQL | Tableau | R

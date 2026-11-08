# DCS: Titanic Passenger Survival Visualization & Analysis

## Overview & Basic Description
This repository contains the hands-on data analytics and visualization assignment evaluating how different chart types influence audience interpretation. 

We analyze the historical RMS Titanic passenger survival distribution, comparing two distinct visual encodings:
1. **A Bar Chart** (representing absolute frequencies and percentages along an aligned common baseline)
2. **A Pie Chart** (representing part-to-whole proportional shares in a 360-degree circle)

---

## Dataset Source
* **Source:** The dataset was taken from the official Kaggle competition: [Titanic - Machine Learning from Disaster](https://www.kaggle.com/competitions/titanic) (`train.csv`).
* **Description:** Contains records for 891 passengers on the RMS Titanic in April 1912.
* **Key Variable:** `Survived` — a binary indicator (`0` = Did Not Survive, `1` = Survived).

---

## Repository Structure

```text
dcs/
├── README.md
└── main assig/
    ├── README.md                          # Detailed assignment documentation
    ├── data/
    │   └── train.csv                      # Titanic dataset from Kaggle (891 records)
    ├── notebooks/
    │   └── titanic_visualization.ipynb    # Jupyter Notebook with data exploration, cleaning & chart generation
    ├── charts/
    │   ├── bar_chart.png                  # High-resolution (300 DPI) Bar Chart
    │   └── pie_chart.png                  # High-resolution (300 DPI) Pie Chart
    └── report/
        ├── titanic_visualization_report.docx  # 1–2 page Word reflection report
        └── titanic_visualization_report.md    # Markdown version of the report
```

---

## Visualizations & Key Findings

From the 891 passengers recorded in `train.csv`:
* **Did Not Survive (Perished):** **549 passengers** (**61.6%**)
* **Survived:** **342 passengers** (**38.4%**)

### Chart 1: Bar Chart (Figure 1)
![Bar Chart](main%20assig/charts/bar_chart.png)

* **Key Strengths:** High perceptual accuracy (Cleveland & McGill Tier 1). Placing categories on a common zero baseline allows instantaneous length comparisons without cognitive fatigue. Both raw counts and percentages are directly visible.

---

### Chart 2: Pie Chart (Figure 2)
![Pie Chart](main%20assig/charts/pie_chart.png)

* **Key Strengths:** Clearly communicates the part-to-whole relationship, emphasizing that casualties formed the majority (>60%) of the cohort.
* **Limitations:** Radial angles and 2D wedge areas are subject to perceptual underestimation, requiring textual labels to read precise counts.

---

## Conclusion
While the pie chart effectively illustrates general majority-minority proportions, the **bar chart is significantly more effective for quantitative communication**. It eliminates angle distortion and enables accurate, rapid comparisons along an aligned metric axis.

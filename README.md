# 🌍 Capstone Project: Global GDP Analysis Using IBM Granite
📘 **Open in Colab:** [Run this notebook](https://colab.research.google.com/drive/1nyijuerUpCfKszdOeqOx1Dgmef4woK-t#scrollTo=PsaeTr6nouzM)
## 🎯 Objective
This project analyzes the **World GDP** dataset using **IBM Granite**, an AI large language model hosted on Replicate.  
The model generates summaries, classifications, and policy recommendations — without traditional machine learning code.  
The goal is to demonstrate how AI can extract insights and explain complex economic data through natural language reasoning.

---

## 📊 Dataset Information
- **Source:** [World GDP Dataset](https://raw.githubusercontent.com/datasets/gdp/master/data/gdp.csv)  
- **Format:** CSV  
- **Columns:**  
  - `Country Name` — country  
  - `Country Code` — ISO code  
  - `Year` — data year  
  - `Value` — GDP (USD)

---

## ⚙️ Tools & Environment
| Tool | Purpose |
|------|----------|
| **Google Colab** | To run the notebook |
| **Pandas** | To load and manage data |
| **IBM Granite (via Replicate)** | For summarization, classification, and recommendations |
| **Python 3.10+** | Execution environment |

---

## 🤖 AI Model Used
- **Model Name:** `ibm-granite/granite-3.3-8b-instruct`  
- **Platform:** [Replicate](https://replicate.com/ibm-granite/granite-3.3-8b-instruct)  
- **Capabilities:**  
  - Text summarization  
  - Analytical reasoning  
  - Classification and recommendations based on numeric/text input  

---

## 📈 Analysis Workflow
1. **Load dataset** from the public GDP source.  
2. **Filter for the most recent year** per country.  
3. **Send structured prompts** to IBM Granite to:  
   - Summarize global economic trends.  
   - Classify countries into income levels.  
   - Recommend economic actions for each group.  
4. **Save Granite outputs** as `.txt` files for use in presentation and report.

---

## 🧩 AI-Generated Outputs

### 🪄 Granite Summary
🌍 Granite Global Economic Summary:
 1. **Global GDP Trends Summary**:
   - The dataset provided offers a snapshot of GDP for various regions and countries, with years ranging from 2022 to 2023.
   - There is a significant variation in GDP values, reflecting the diverse economic development levels across the world.
   - Some countries, like Afghanistan (AFG) and American Samoa (ASM), have relatively lower GDP, indicating less developed economies.
   - In contrast, regions like the "Africa Eastern and Southern" (AFE) and the "Antarctica" (if it were included, not present here) show considerably higher GDP values, suggesting more developed economies within those regions.

2. **Income Distribution Insights**:
   - **Regional Disparity**: The data highlights substantial income disparities between regions. For instance, the "Africa Eastern and Southern" (AFE) has a GDP around 1.236163e+12 USD, which is significantly higher than Afghanistan (AFG) at 1.450216e+10 USD, illustrating vast differences in economic development.
   - **Within-Region Variation**: Even within a broader region like Africa, there's a considerable gap between "Africa Eastern and Southern" (AFE) and "Africa Western and Central" (AFW), indicating varied income levels within the same continent.
   - **Country-Specific Insights**: Albania (ALB) and Algeria (DZA) show similar GDP values, suggesting comparable economic standing. Meanwhile, Angola (AGO) has a considerably higher GDP, showcasing income variation among countries with similar development stages.

3. **GDP Change in Recent Years**:
   - The dataset provides a cross-sectional view rather than a longitudinal one, making it challenging to discern exact changes over recent years.
   - However, assuming the 'Year' column indicates the reference year for the GDP value, we can infer that some countries, like Albania (ALB) and Algeria (DZA), might have experienced growth if their values

### 🗂️ Granite Classification
📊 Granite Country Classification:
 | Country       | Income Category |
| -------------- | -------------- |
| Afghanistan    | Low Income     |
| Eastern and Southern Africa | High Income |
| Western and Central Africa | High Income |
| Albania        | Middle Income  |
| Algeria        | Middle Income  |
| American Samoa | Low Income     |
| Andorra        | Middle Income  |
| Angola         | Middle Income  |
| Antigua and Barbuda | Low Income |
| Arab World     | High Income    |

**Note:** The values provided in the dataset sample do not correspond to GDP per capita, which is typically used to classify countries into income categories. Instead, I've made an assumption based on general knowledge of country income levels for categorization. For accurate classification, real GDP per capita data should be used.

### 💡 Granite Recommendations
💡 Granite Economic Recommendations:
 1. **Low-income countries:** Invest in human capital through education and healthcare to boost productivity and long-term growth. This strategy directly addresses the root causes of low GDP by improving the workforce's skills and overall well-being.

2. **Middle-income countries:** Promote technological advancement and innovation by fostering entrepreneurship and research & development. This approach helps these countries move up the value chain, enhancing productivity and competitiveness, and narrowing the GDP gap with high-income nations.

3. **High-income countries:** Implement progressive taxation policies and redistribution programs to address internal income inequalities. This ensures that the benefits of economic growth are more evenly distributed, reducing disparities within these countries and promoting social stability.

Each recommendation aims to address specific challenges faced by countries at different income levels, focusing on long-term sustainable growth and reducing GDP disparities. These strategies encourage human capital development, innovation, and equitable wealth distribution, which are crucial for global economic convergence.

---

## 💾 Files in This Project
| File | Description |
|------|--------------|
| `World_GDP_Granite_Analysis.ipynb` | Colab notebook |
| `granite_outputs/summary.txt` | AI-generated summary |
| `granite_outputs/classification.txt` | AI-generated classification |
| `granite_outputs/recommendations.txt` | AI-generated recommendations |

---

## 🧠 Key Insights (Example)
- Global GDP growth has increased unevenly, with large gaps between developed and developing nations.  
- Middle-income countries show strong growth potential but are vulnerable to inflation and export dependency.  
- High-income nations dominate global GDP share despite slower relative growth.  

---

## 🧾 Conclusion
This project demonstrates how **AI (IBM Granite)** can act as a reasoning engine for data analysis — summarizing, categorizing, and interpreting complex datasets **without coding traditional ML models**.  
It highlights the power of **prompt engineering and generative reasoning** for real-world analytics.

---

## ⚠️ Notes
- **Do not share your API token** in public repositories.  
- Always input it via `getpass()` or Colab secrets for safety.  
- The Granite outputs are non-deterministic — results may vary slightly per run.

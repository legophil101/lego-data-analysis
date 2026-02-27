# 🧱 LEGO Market Evolution Analysis (1949–2021)

## 📌 Executive Overview

This project delivers a **longitudinal, data-driven analysis** of LEGO’s product catalog and manufacturing history. By systematically exploring the Rebrickable database, it uncovers the strategic decisions that allowed LEGO to evolve from a niche toy manufacturer into a global entertainment powerhouse.

Key focus areas include **market segmentation, product premiumization, and licensing strategy**, highlighting how LEGO navigated growth plateaus in the 1990s and captured the **Adult Fan of LEGO (AFOL) market**.

---

## 🔍 Analytical Objectives

1. **Production Volume Trends:** Quantify the scale and pace of LEGO set releases over 70+ years.
2. **Thematic Diversification:** Examine whether growth is driven by depth (more sets per theme) or breadth (new themes).
3. **Product Premiumization:** Track average part counts to reveal the shift toward high-complexity builds.
4. **Franchise Dominance:** Resolve relational data to identify which licensed IPs drive the highest production volumes.

---

## 🚀 Technical Highlights

* **Relational Data Modeling:** Merged `sets.csv` and `themes.csv` via foreign keys to maintain **relational integrity** and translate raw IDs into readable theme names.
* **Data Integrity Management:** Excluded incomplete reporting periods (2020–2021) to ensure trend reliability.
* **Advanced Aggregation:** Applied `.agg()`, `.nunique()`, and multi-level grouping to analyze 15,000+ records efficiently.
* **Professional Visualizations:** Dual-axis time-series and bar charts highlight correlations between production volume, theme diversity, and average set complexity.
* **Asset Integration:** Included visual references (`assets/`) for thematic trends, Rebrickable schema, and product imagery.

---

## 📊 Key Business Insights

* **1990s Inflection Point:** A sharp increase in both sets and themes aligns with LEGO’s adoption of **licensed IP partnerships** (Star Wars, Harry Potter).
* **Premiumization Strategy:** Average part counts per set rose significantly, demonstrating a deliberate pivot toward **high-margin, adult-oriented products**.
* **Franchise Dominance:** Relational merging confirms **Star Wars** as LEGO’s highest-volume franchise, validating long-term licensing as a growth engine.
* **Strategic Pillars of Growth:**

  * **Thematic Innovation:** Expansion into diverse categories captures new demographics.
  * **Premium Products:** Complexity drives collector engagement and revenue.
  * **IP Licensing:** Partnerships accelerate scale and brand resonance.

---

## 🛠 Tools & Environment

* **Python 3.x** – Core programming language
* **Pandas** – Data cleaning, aggregation, and relational merging
* **Matplotlib** – Professional-grade time-series and categorical visualizations
* **Jupyter Notebook** – Integrated exploratory analysis and narrative reporting

---

## 🗂 Repository Structure

```text
lego-data-analysis/
├── assets/                   # Visuals and charts for analysis
│   ├── bricks.jpg
│   ├── lego_sets.png
│   ├── lego_themes.png
│   └── rebrickable_schema.png
├── data/                     # Raw Rebrickable CSVs
│   ├── colors.csv
│   ├── sets.csv
│   └── themes.csv
├── notebooks/                # Main analytical notebook
│   └── lego_data_analysis.ipynb
├── .gitignore                # Hide local venv/cache files from GitHub
├── README.md                 # Project documentation
└── requirements.txt          # Project dependencies
```

> ⚠ `.ipynb_checkpoints/` and `.venv/` are **ignored in GitHub** via `.gitignore`

---

## ▶️ How to Run

1. **Clone the repository:**

   ```bash
   git clone https://github.com/legophil101/lego-data-analysis.git
   ```
2. **Install dependencies:**

   ```bash
   pip install -r requirements.txt
   ```
3. **Launch Jupyter Notebook:**

   ```bash
   python -m notebook
   ```
4. **Open the analysis:**
   
   `notebooks/lego_data_analysis.ipynb`

---

## 📚 Data Source

Analysis based on the **Rebrickable LEGO Database**, using relational tables for colors, themes, and sets.
[Access Data Here](https://rebrickable.com/downloads/)

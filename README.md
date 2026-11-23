# ☕ Starbucks Nutrition Insights Dashboard

An interactive Power BI dashboard analyzing Starbucks beverage nutrition data across categories, individual beverages, and protein/beverage filters. Built to compare **Calories**, **Caffeine**, **Sugar**, and **Protein** across the beverage lineup so consumers and analysts can quickly spot high-calorie, high-sugar, high-caffeine, and protein-rich options.

---

## 🖼️ Dashboard Preview

<p align="center">
  <img src="Dashboard%20Screenshot.png" alt="Starbucks Nutrition Insights Dashboard" width="50%">
</p>

### Key Visual Components in `Starbucks-analysis.pbix`
* **Top KPI Cards:** `Total Beverages`, `Avg Calories`, `Avg Sugar`, and `Avg Caffeine`.
* **Interactive Filters (Slicers):** Filter by **Beverage** (`starbucks.Beverage`) and **Protein (g)** (`starbucks. Protein (g) `).
* **Category & Beverage Visuals:**
  * **Line Chart:** Sum of `Calories` by `Beverage_Category`.
  * **Column Chart:** Sum of `Calories` by `Beverage` (filtered to Top 6).
  * **Donut Chart:** `Total Beverages` distribution by `Beverage_Category` across 9 beverage categories.
  * **Bar Chart:** `Avg Caffeine` by `Beverage` (filtered to Top 5).
  * **Area Chart:** `Avg Caffeine` by `Beverage_Category` (filtered to Top 5).

---

## 🧪 Nutritional Metrics Analysis

### 1. Calories (`Calories` & `Avg Calories`)
* Tracks total energy contribution and average energy across beverage categories and individual drinks.
* Helps distinguish low-calorie brewed coffees and teas from calorie-dense blended, cream-, or syrup-heavy drinks.

### 2. Caffeine (`Avg Caffeine`)
* Evaluates average caffeine content across individual beverages (bar chart) and beverage categories (area chart), alongside the headline `Avg Caffeine` KPI card.
* Useful for comparing espresso- and coffee-based beverages against lower-caffeine or caffeine-free blended/specialty options.

### 3. Sugar (`Avg Sugar`)
* Monitors average sugar content via a dedicated top-level KPI card.
* Highlights how added syrups, sauces, and sweet bases drive sugar load across menu items.

### 4. Protein (`Protein (g)`)
* Included as an interactive between-range filter (`starbucks. Protein (g) `) in the report header so users can slice and inspect beverages by gram protein levels (0 g to 20 g).
* Typically correlates with milk-based or specialty/smoothie formulations compared with straight black coffee or plain tea.

---

## 📊 Key Findings & Structure

* **Dataset & Categories:** Covers **242** beverage records (**218** clean rows) across **18** columns and **9** beverage categories (*Classic Espresso Drinks*, *Tazo® Tea Drinks*, *Frappuccino® Blended Coffee*, etc.).
  Paired with four KPI cards (`Total Beverages`, `Avg Calories`, `Avg Sugar`, `Avg Caffeine`) and `Beverage` / `Protein (g)` (`0 g – 20 g`) slicers.
* **Calories (3 – 510 kcal):** Ranges from **3 kcal** (*Brewed Coffee* – Short) up to **510 kcal** across the dataset.
  The column chart highlights the **Top 6** high-calorie drinks (axis capped at **350**), including *White Chocolate Mocha* and *Java Chip* (without whipped cream).
* **Sugar & Milk Impact (0 g – 84 g):** Sugars span **0 g – 84 g**, shifting noticeably with cup size and milk selection.
  For example, *Caffè Latte* moves from **70 kcal** (**9 g** sugar, **6 g** protein) in Short Nonfat Milk to **150 kcal** (**14 g** sugar, **10 g** protein) in Tall 2% Milk.
* **Caffeine (0 mg – 410 mg):** Ranges from **0 mg** up to **410 mg** (Venti *Brewed Coffee* at **410 mg**, Grande **330 mg**, Tall **260 mg**, Short **175 mg**).
  The bar and area charts focus on the **Top 5** beverages and **Top 5** categories by `Avg Caffeine`.

---

## 📂 Dataset Source

* **Source:** Starbucks Beverage Nutrition Dataset (commonly sourced from Kaggle's *Starbucks Nutrition* / *Starbucks Drink Nutrition* datasets, using the `starbucks` table containing fields such as `Beverage_Category`, `Beverage`, `Calories`, and `Protein (g)`).
* **Project File:** `Starbucks-analysis.pbix` (Power BI report with `Measures (2)` and `starbucks` data model).

---

## 🛠️ Tools Used
* **Microsoft Power BI** (Data modeling, DAX measures in `Measures (2)`, interactive slicers, and charts)
* **GitHub** (`ChandanShetty06/Starbucks-Nutrition-Insights-Dashboard`)

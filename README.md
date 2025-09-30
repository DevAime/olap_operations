
Aime Muganga-232
---

# OLAP Demo

This project demonstrates **basic OLAP (Online Analytical Processing) operations** using Python with **pandas**, **SQLite**, and **seaborn** for visualization.
It covers the three OLAP models:

* **ROLAP** (Relational OLAP) → SQL-based aggregations
* **MOLAP** (Multidimensional OLAP) → In-memory pivot tables
* **HOLAP** (Hybrid OLAP) → Combination of ROLAP and MOLAP

The script also demonstrates common OLAP operations like **slice, dice, drill-down, and roll-up**.

---

## Features

* Create and load sample employee and department data into SQLite.
* Perform **ROLAP** aggregations using SQL queries.
* Perform **MOLAP** analysis with pandas pivot tables.
* Perform **HOLAP** analysis combining SQL and pandas.
* Visualize results using bar plots and heatmaps.
* Demonstrate **slice, dice, drill-down, and roll-up** operations.

---

## Requirements

Make sure you have the following installed:

* Python 3.x
* pandas
* numpy
* sqlite3 (comes with Python)
* seaborn
* matplotlib

You can install the Python libraries with:

```bash
pip install pandas numpy seaborn matplotlib
```

---

## Usage

1. Clone this repository or copy the script.
2. Run the script:

```bash
python olap_demo.py
```

3. The script will:

   * Create a SQLite database (`olap_demo.db`).
   * Populate it with sample employee and department data.
   * Perform OLAP operations (ROLAP, MOLAP, HOLAP).
   * Display results in the console and as plots.

---

## Example Outputs

* **ROLAP:** Average salary by department (SQL aggregation).
* **MOLAP:** Salary cube (Department × Age).
* **HOLAP:** Summary of average salaries combining SQL and pandas.
* **Slice/Dice/Drill-down/Roll-up:** Additional OLAP operations with visualizations.


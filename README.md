
Aime Muganga-232
---

# OLAP Demo

This notebook demonstrates basic OLAP (Online Analytical Processing) operations using Python with pandas, SQLite, and seaborn for visualization.


## What is OLAP?

**OLAP (Online Analytical Processing)** is a category of tools and techniques that allows users to analyze large volumes of data quickly and interactively. Unlike traditional databases that focus on day-to-day transactions (**OLTP – Online Transaction Processing**), OLAP is optimized for answering analytical queries such as:

* What is the average salary by department?
* How does salary vary across different age groups?
* Can we compare totals across multiple dimensions?

OLAP works with **multidimensional data (cubes)**, enabling operations such as:

* **Roll-up** → Summarizing data at a higher level (e.g., total salary by department).
* **Drill-down** → Looking at more detailed levels (e.g., salary by individual employees).
* **Slice** → Filtering data on a single dimension (e.g., only HR department).
* **Dice** → Filtering on multiple conditions (e.g., HR employees with salary > 60,000).

There are three main OLAP models:

* **ROLAP (Relational OLAP):** Uses relational databases (SQL queries).
* **MOLAP (Multidimensional OLAP):** Uses in-memory cubes and pivot tables.
* **HOLAP (Hybrid OLAP):** Combines ROLAP + MOLAP for flexibility.

This notebook demonstrates all three approaches with visual examples.

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

Open the notebook in Jupyter:

jupyter notebook olap_operations.ipynb

Run all cells to:

* Create a SQLite database (olap_demo.db).

*Insert sample employee & department data.

*Perform ROLAP, MOLAP, HOLAP operations.

*Generate visualizations for each OLAP operation.

---

## Example Outputs

ROLAP: Average Salary by Department
<img width="500px" alt="image" src="https://github.com/user-attachments/assets/cb7e0286-b173-474a-b252-4cbb41b45f52" />


MOLAP: Average Salary Cube (Department vs Age)
<img width="500px" alt="image" src="https://github.com/user-attachments/assets/a8937611-41de-4b10-9f2e-47eb53177314" />


HOLAP: Average Salary by Department
<img width="500px" alt="image" src="https://github.com/user-attachments/assets/f71d3224-3b82-486e-adbc-adeda39f9877" />


Drill-down: Salary by Employee and Department
<img width="500px" alt="image" src="https://github.com/user-attachments/assets/9b14e34b-db97-4b1d-a4ae-a59265a1fac6" />


Roll-up: Total Salary by Department
<img width="500px" alt="image" src="https://github.com/user-attachments/assets/f1673777-588d-4473-b6bf-7ee38107f73c" />

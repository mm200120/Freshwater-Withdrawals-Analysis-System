# Freshwater-Withdrawals-Analysis-System

## Overview

The **Freshwater Withdrawals Analysis System (FWAS)** is a data analysis and visualization project designed to explore, analyze, and compare freshwater withdrawal trends across countries and over time. The system processes structured freshwater withdrawal datasets and provides insights through statistical analysis and interactive visualizations.

This project is suitable for **environmental research, water resource management, policy analysis, and academic studies**, particularly in sustainability and climate-related fields.

---

## Objectives

* Analyze freshwater withdrawal trends by **country and year**
* Compare water usage patterns between multiple countries
* Identify long-term trends and anomalies
* Generate publication-ready visualizations
* Export cleaned and structured data for further research

---

## Key Features

* Modular **data loading and preprocessing**
* Country-level and multi-country trend analysis
* Time-series visualizations (static and interactive)
* Research-ready data exports
* Designed for extensibility and reuse

---

## Technologies Used

* **Python 3**
* **pandas** – data manipulation and analysis
* **numpy** – numerical computations
* **matplotlib & seaborn** – static visualizations
* **plotly** – interactive visualizations
* **Jupyter Notebook** – development and presentation environment

---

## Project Structure

```
FWAS/
│
├── Freshwater Withdrawals Analysis System (FWAS).ipynb
├── README.md
└── (exported datasets)
```

---

## System Workflow

### 1. Setup and Dependencies

The notebook begins by installing and importing all required libraries to ensure a reproducible environment.
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/3b710cfe-229a-4e07-9fe9-40c79dba21b6" />

### 2. Data Loading

A dedicated class (`FreshwaterDataLoader`) is responsible for:

* Loading freshwater withdrawal datasets
* Cleaning missing or inconsistent values
* Transforming data into **long format** suitable for time-series analysis

### 3. Data Processing

The system:

* Filters data by country and year
* Normalizes and structures indicators
* Prepares datasets for visualization and export
  
  <img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/0517d808-7376-46fa-809c-8ceb0b7a906d" />


### 4. Analysis Functions

Key analytical capabilities include:

* Single-country trend analysis
* Cross-country comparisons
* Temporal analysis across defined year ranges

Example:

```python
analyze_country('Botswana', loader.df_long)
```
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/eba484cf-d0b2-45ec-9e76-d6316d1731af" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/f832ead2-4126-48c4-9f18-464b5f33646a" />

### 5. Visualization

FWAS supports both static and interactive plots:

* Line charts for trend analysis
* Multi-country comparison graphs
* Interactive Plotly figures for exploration

Example:

```python
plot_country_trend(['Botswana', 'South Africa', 'Zimbabwe'], df, 1990, 2020)
```

---

## Data Export

The system includes an export utility that:

* Saves processed datasets in research-friendly formats
* Automatically timestamps exported files
* Enables reuse in external tools (R, Excel, GIS, etc.)
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/6b25825b-4662-4988-b2c1-098195daabd5" />

---

## Use Cases

* Academic research in water resource management
* Environmental impact assessments
* Policy and development planning
* Comparative regional water studies
* Educational demonstrations
  
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e2e8741d-3535-4952-aabb-24a42ee4fa9e" />

---

## Example Countries Analyzed

* Botswana
* South Africa
* Zimbabwe
* Nigeria
* United States

(Expandable to any country present in the dataset)

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/cf2fd898-2380-4560-be29-b40e9000c955" />

---

## How to Run

1. Open the notebook in Jupyter
2. Run all cells sequentially
3. Modify country names or year ranges as needed
4. Export or visualize results

---

## Future Improvements

* Integration with real-time data sources (World Bank API)
* Per-capita water withdrawal analysis
* Sectoral breakdown (agriculture, industry, domestic)
* Forecasting using machine learning models
* Web dashboard deployment

---

## Author

**Maatla Ookeditse Mosimanyane**

---

## License

This project is intended for **academic and research use**. Licensing can be added based on institutional or publication requirements.

---

*FWAS aims to support data-driven decision-making for sustainable water management.*

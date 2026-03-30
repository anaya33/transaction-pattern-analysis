<div align="center">

# Transaction Pattern Analysis

**A Data-Driven Analysis of Temporal Sales Dynamics and Demand Peaks**

[![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![Contributions Welcome](https://img.shields.io/badge/Contributions-Welcome-brightgreen?style=for-the-badge)](#contributing)

[View Notebook](#notebook) · [Dataset](#dataset) · [Results](#results) · [Contributing](#contributing)

</div>

---

## Overview

This project investigates **temporal purchasing behavior** within a retail bakery environment using transactional sales data. The objective is to identify patterns in customer demand across time and evaluate how these patterns can inform operational decision-making.

The analysis provides insight into how temporal dynamics influence retail performance and demonstrates how data-driven approaches can support optimization of:
- **Inventory management**
- **Staffing allocation**
- **Production scheduling**

---

## Features

| Category | Techniques |
|----------|------------|
| **Data Preprocessing** | Cleaning, type conversion, missing value handling |
| **Feature Engineering** | Time-based feature extraction (hourly segmentation) |
| **Exploratory Analysis** | Distribution analysis, correlation matrices, trend visualization |
| **Statistical Testing** | Relationship analysis between price, quantity, and time |
| **Clustering** | K-Means (manual implementation + scikit-learn) |
| **Classification** | K-NN (manual implementation + scikit-learn) |
| **Dimensionality Reduction** | Principal Component Analysis (PCA) |

---

## Project Structure

```
transaction-pattern-analysis/
├── transaction_pattern_analysis.ipynb  # Main analysis notebook
├── Bakery sales.csv                    # Raw dataset (234,005 transactions)
├── Bakery_Sales1.json.zip              # JSON export
└── README.md                           # Project documentation
```

---

## Dataset

The dataset contains **234,005 transactional records** from a French retail bakery spanning from January 2021 to September 2022.

| Field | Description |
|-------|-------------|
| `date` | Transaction date |
| `time` | Transaction time (HH:MM) |
| `ticket_number` | Unique transaction identifier |
| `article` | Product name |
| `Quantity` | Number of items purchased |
| `unit_price` | Price per unit (€) |

**Source:** [Kaggle - French Bakery Daily Sales](https://www.kaggle.com/datasets/matthieugimbert/french-bakery-daily-sales)

> **Note:** Data cleaning is performed directly within the notebook to ensure transparency and reproducibility.

---

## Results

### Sales Distribution by Hour
The analysis reveals clear peak demand periods throughout the day, enabling targeted staffing and inventory decisions.

```
Peak Hours: Morning rush (8-10 AM) and afternoon (12-2 PM)
```

### Clustering Analysis
K-Means clustering segments transactions into distinct behavioral groups based on quantity and pricing patterns.

### PCA Insights
Principal Component Analysis reduces dimensionality while preserving variance, revealing underlying structure in transaction data.

---

## Tech Stack

<div align="center">

| Tool | Purpose |
|------|---------|
| ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) | Core programming language |
| ![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white) | Data manipulation & analysis |
| ![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white) | Numerical computing |
| ![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=flat-square) | Data visualization |
| ![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=flat-square) | Statistical visualization |
| ![scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white) | Machine learning |

</div>

---

## Getting Started

### Prerequisites

- Python 3.8+
- Jupyter Notebook or Google Colab

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/anaya33/transaction-pattern-analysis.git
   cd transaction-pattern-analysis
   ```

2. **Install dependencies**
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```

3. **Launch the notebook**
   ```bash
   jupyter notebook transaction_pattern_analysis.ipynb
   ```

### Using Google Colab

1. Open [Google Colab](https://colab.research.google.com/)
2. Upload `transaction_pattern_analysis.ipynb`
3. Upload `Bakery sales.csv` or connect via GitHub
4. Run cells sequentially

---

## Contributing

Contributions are welcome! Here's how you can help:

### Ways to Contribute

- **Bug Reports** — Found an issue? Open a detailed bug report
- **Feature Requests** — Have ideas for new analyses? Share them!
- **New Visualizations** — Add compelling charts or dashboards
- **Additional ML Models** — Implement other clustering/classification algorithms
- **Documentation** — Improve explanations or add tutorials
- **Code Optimization** — Enhance performance or code quality

### Contribution Guidelines

1. **Fork** the repository
2. **Create** a feature branch
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. **Commit** your changes with clear messages
   ```bash
   git commit -m "Add: description of your changes"
   ```
4. **Push** to your branch
   ```bash
   git push origin feature/your-feature-name
   ```
5. **Open** a Pull Request with a detailed description

### Ideas for Contributors

| Difficulty | Task |
|------------|------|
| Easy | Add more visualizations (box plots, violin plots) |
| Easy | Improve code comments and documentation |
| Medium | Implement DBSCAN or hierarchical clustering |
| Medium | Add time series forecasting (ARIMA, Prophet) |
| Medium | Create an interactive dashboard (Plotly/Dash) |
| Advanced | Build a recommendation system for products |
| Advanced | Deploy as a web application |

---

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

- Dataset provided by [Matthieu Gimbert on Kaggle](https://www.kaggle.com/datasets/matthieugimbert/french-bakery-daily-sales)
- Developed as part of **Advanced Data Analytics (ITEC 4220)** coursework

---

<div align="center">

**Star this repo if you found it helpful!**

[View Live Project](https://anaya33.github.io/transaction-pattern-analysis/) · [Download JSON Data](./Bakery_Sales1.json.zip)

</div>



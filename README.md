# 🐼 Pandas – Basics for Beginners
A beginner-friendly collection of **Pandas** code examples covering all the essential concepts you need to start working with data in Python. Clean, well-commented, and easy to follow.

---

## 📚 Table of Contents

- [About](#-about)
- [Getting Started](#-getting-started)
- [Topics Covered](#-topics-covered)
- [Folder Structure](#-folder-structure)
- [Requirements](#-requirements)
- [How to Use](#-how-to-use)
- [Contributing](#-contributing)
- [License](#-license)

---

## 📖 About

This repository is a hands-on reference guide for the **Pandas** library in Python. It focuses on the core fundamentals — the building blocks every data analyst and Python developer needs. Each script is well-commented and self-contained, making it easy to learn and experiment.

---

## 🚀 Getting Started

```bash
# Clone the repository
git clone https://github.com/your-username/pandas-repo.git
cd pandas-repo

# Install dependencies
pip install -r requirements.txt
```

---

## 📂 Topics Covered

| File | Topic | What You'll Learn |
|------|-------|-------------------|
| `01_series.py` | Pandas Series | Creating, indexing, and operating on Series |
| `02_dataframe_creation.py` | DataFrame Basics | Creating DataFrames from dicts, lists, and CSVs |
| `03_reading_writing.py` | File I/O | Reading/writing CSV, Excel, and JSON files |
| `04_viewing_data.py` | Exploring Data | `head()`, `tail()`, `info()`, `describe()`, `shape` |
| `05_indexing_selection.py` | Selecting Data | Column selection, `loc`, `iloc` |
| `06_filtering.py` | Filtering Rows | Boolean conditions and multiple filters |
| `07_sorting.py` | Sorting | Sorting by columns, index, ascending/descending |
| `08_handling_nulls.py` | Missing Data | `isnull()`, `dropna()`, `fillna()` |
| `09_adding_columns.py` | Modifying DataFrames | Adding, renaming, and dropping columns |
| `10_basic_stats.py` | Statistics | `mean()`, `sum()`, `count()`, `min()`, `max()`, `value_counts()` |

```python
import pandas as pd

# Create a DataFrame
df = pd.DataFrame({
    'Name': ['Alice', 'Bob', 'Charlie'],
    'Age':  [25, 30, 35],
    'City': ['New York', 'London', 'Tokyo']
})

# View basic info
print(df.describe())

# Filter rows
print(df[df['Age'] > 28])

# Handle missing values
df['Score'] = [90, None, 85]
df['Score'].fillna(df['Score'].mean(), inplace=True)
```

---

## 🗂️ Folder Structure

```
pandas-repo/
│
├── 01_Basic.ipynb
├── 02_dataframe_creation.ipynb
├── 03_reading_writing.ipynb
├── 04_viewing_data.ipynb
├── 05_indexing_selection.ipynb
├── 06_filtering.ipynb
├── 07_sorting.ipynb
├── 08_handling_nulls.ipynb
├── 09_adding_columns.ipynb
├── 10_basic_stats.ipynb
│
├── datasets/
│   └── sample_data.csv
│
├── requirements.txt
└── README.md
```

---

## 📦 Requirements

```
pandas>=1.5.0
numpy>=1.21.0
openpyxl>=3.0.0
matplotlib>=3.5.0
jupyter>=1.0.0
```

Install all at once:

```bash
pip install -r requirements.txt
```

---

## 🛠️ How to Use

1. Browse the folders (`basic/`, `intermediate/`, `advanced/`) based on your level.
2. Run any script directly:
   ```bash
   python basic/02_dataframe_creation.py
   ```
3. Or open notebooks in Jupyter:
   ```bash
   jupyter notebook
   ```

---

## 🤝 Contributing

Contributions are welcome! If you want to add new examples or fix issues:

1. Fork the repository
2. Create a new branch: `git checkout -b feature/your-topic`
3. Commit your changes: `git commit -m "Add: topic description"`
4. Push to the branch: `git push origin feature/your-topic`
5. Open a Pull Request

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---


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
| `01.Basic.ipynb` | Pandas Basics | Introduction to Pandas, Series, and basic operations |
| `02.Data_frames.ipynb` | DataFrames | Creating and working with DataFrames |
| `03.Data_frames_function.ipynb` | DataFrame Functions | Exploring useful DataFrame functions and methods |
| `04.Groupby_objects.ipynb` | GroupBy Operations | Grouping, aggregating, and analyzing data |
| `05.Merging_joining_concatenating.ipynb` | Merge, Join & Concatenation | Combining multiple DataFrames using merge, join, and concat |
| `06.Multiindex.ipynb` | MultiIndex | Working with hierarchical indexing in Pandas |
| `07.Long_vs_Wide_data.ipynb` | Long vs Wide Data | Understanding and reshaping long and wide data formats |
| `08.vectorized_operation.ipynb` | Vectorized Operations | Performing fast and efficient operations on data |
| `09.Timestamp_objects.ipynb` | Timestamp Objects | Working with timestamps and date-time values |
| `10.datetimeIndex_object.ipynb` | DateTimeIndex Object | Handling and indexing time-series data using DateTimeIndex |
``
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
# 📊 Pandas Repository

## 🗂️ Folder Structure

```bash
pandas-repo/
│
├── 1.Basic.ipynb
├── 2.Dataframes.ipynb
├── 3.dataframe_function.ipynb
├── 4.Groupby_objects.ipynb
├── 5.merger_joining_concatation.ipynb
├── 6.Multiindex.ipynb
├── 7.Long_vs_Wide_data.ipynb
├── 8.vectorized_operation.ipynb
├── 9.Timestamp_objects.ipynb
├── 10.datetimeIndex_object.ipynb
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


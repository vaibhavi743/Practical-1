# 📚 Library Transaction Data Analysis

> A Python-based data analysis project for analyzing library borrowing transactions, identifying borrowing patterns, performing statistical analysis, and generating meaningful visualizations.

---

## 📌 Project Overview

The **Library Transaction Data Analysis** project analyzes library borrowing records using Python and popular data analysis and visualization libraries.

The project focuses on understanding borrowing behavior through data validation, transaction filtering, statistical analysis, aggregation, duplicate handling, and visual exploration.

The complete analysis is implemented in a Jupyter Notebook using a structured `DataAnalysis` class.

---

## 🎯 Project Objectives

The main objectives of this project are to:

- Load and validate library transaction data
- Check the dataset for missing values
- Filter transactions based on conditions
- Generate a library transaction report
- Calculate borrowing duration statistics
- Analyze transactions by genre
- Analyze book-wise borrowing activity
- Handle duplicate records
- Identify the most borrowed books
- Analyze monthly borrowing trends
- Visualize genre-wise borrowing distribution
- Visualize borrowing activity using a heatmap

---

## 📊 Dataset

**Dataset:** `library_transaction.csv`

### Dataset Columns

| Column | Description |
|---|---|
| `TransactionID` | Unique identifier for each transaction |
| `Date` | Date of the library transaction |
| `User_ID` | Unique identifier of the library user |
| `Book_Title` | Name of the borrowed book |
| `Genre` | Genre/category of the book |
| `Borrowing_Duration_Days` | Number of days the book was borrowed |

---

## 🛠️ Technologies & Libraries

- **Python**
- **Pandas** – Data loading, cleaning and analysis
- **NumPy** – Numerical and statistical calculations
- **Matplotlib** – Data visualization
- **Seaborn** – Statistical visualization
- **Jupyter Notebook** – Development environment

---

# 🔎 Project Workflow

## 1. Data Input & Validation

The dataset is loaded using Pandas.

```python
df = pd.read_csv("library_transaction.csv")

The project also checks for missing values using:

df.isnull().sum()

The dataset contains no missing values in the displayed validation results.

2. Library Management & Transaction Analysis

A DataAnalysis class is used to organize the analysis operations.

Data Loading

The load_data() method loads the CSV file and stores it for further analysis.

Transaction Filtering

Transactions can be filtered using conditions.

Example:

obj.filter_transaction("Borrowing_Duration_Days > 10")

This helps identify transactions where books were borrowed for more than 10 days.

Transaction Report

The project generates a summary report containing:

Total Transactions
Total Users
Total Books
Average Borrowing Duration
Report Summary
Metric	Value
Total Transactions	150
Total Users	50
Total Books	15
Average Borrowing Duration	16.19 days

📈 Data Analysis & Computations

Borrowing Duration Statistics
Statistical analysis is performed on Borrowing_Duration_Days.
The project calculates:
Mean
Median
Minimum
Maximum
Standard Deviation
Results
Statistic	Value
Mean	16.19
Median	16
Minimum	3
Maximum	30
Standard Deviation	8.62

📚 Genre-wise Analysis

Transactions are grouped according to book genre to understand borrowing patterns across different categories.

📖 Book-wise Aggregation

The project analyzes individual books and calculates:

Total number of borrowings
Average borrowing duration

This helps identify frequently borrowed books and understand their borrowing duration.

♻️ Duplicate Data Handling

Duplicate records are checked and removed to maintain data quality.

df.duplicated().sum()

Duplicates can be removed using:

df = df.drop_duplicates()

📊 Data Visualizations

The project includes multiple visualizations to make the analysis easier to understand.

1. 📊 Bar Chart — Top 5 Most Borrowed Books

Displays the five books with the highest number of borrowing transactions.

top_5_books = df["Book_Title"].value_counts().head(5)

Purpose: Identify the most popular books in the library.

2. 📈 Line Graph — Borrowing Trend Over Months

Shows the number of borrowing transactions across different months.

Purpose: Understand monthly borrowing patterns and trends.

3. 🥧 Pie Chart — Distribution of Books Borrowed by Genre

Displays the proportion of borrowed books belonging to different genres.

Purpose: Understand which genres contribute most to library borrowing activity.

4. 🔥 Heatmap — Borrowing Activity

A heatmap is used to visually represent borrowing activity across time-based categories.

Purpose: Quickly identify areas with higher or lower borrowing activity.

🚀 How to Run the Project
1. Clone the Repository
git clone <your-repository-link>
2. Open the Project

Open the project folder in VS Code or Jupyter Notebook.

3. Install Required Libraries
pip install pandas numpy matplotlib seaborn
4. Open the Notebook
practical 1.ipynb
5. Run the Notebook

Run the cells sequentially from beginning to end.

Make sure that:

library_transaction.csv

is present in the same project folder as the notebook.

💡 Key Insights

This project demonstrates how library transaction data can be used to:

Understand borrowing behavior
Identify popular books
Compare different book genres
Analyze monthly borrowing trends
Calculate borrowing-duration statistics
Perform data cleaning and validation
Detect and handle duplicate records
Convert raw transaction data into meaningful visual insights

🎓 Skills Demonstrated
Python Programming
Object-Oriented Programming
Data Loading
Data Validation
Data Cleaning
Pandas Data Analysis
NumPy Statistical Analysis
Data Aggregation
GroupBy Operations
Duplicate Handling
Data Visualization
Matplotlib
Seaborn
Jupyter Notebook

👩‍💻 Author

Vaibhavi Khokhani

Python & AI Fresher | BCA Graduate

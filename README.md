# Apps Market Analysis with Python

A comprehensive data analysis project exploring Google Play Store and iOS app datasets using **user-defined Python functions** for cleaning, exploration, and interpretation.

## 📊 Project Overview

This project analyzes mobile app market trends by examining:
- **Google Play Store Dataset**: Android app metrics including ratings, reviews, installs, and categories
- **iOS Dataset**: Apple app ecosystem data (extensible for future analysis)

The analysis uses custom Python functions to perform data cleaning, exploratory data analysis (EDA), and statistical insights without relying solely on external libraries.

## 🎯 Key Features

- **Data Cleaning**: 
  - Removal of duplicate entries (keeping records with maximum reviews)
  - Identification and filtering of malformed rows
  - Language filtering (English vs. non-English apps)
  
- **Data Exploration**:
  - Frequency analysis by category and install counts
  - Custom visualization functions
  - Statistical metrics calculation

- **Market Insights**:
  - Most popular app categories
  - Average installation rates by category
  - Free vs. paid app distribution
  - Content rating analysis

## 📈 Analysis Highlights

### Top App Categories (by percentage)
- **Family**: 18.9%
- **Game**: 9.7%
- **Tools**: 8.5%
- **Business**: 4.6%

### Highest Average Installs
- **Communication**: 38.5M average installs
- **Video Players**: 24.7M average installs
- **Social**: 23.3M average installs

## 🗂️ Project Structure

```
apps-market-analysis-with-python/
├── playstoreAnalysis.ipynb    # Main Jupyter Notebook with analysis
├── README.md                   # This file
├── license.txt                 # Creative Commons Attribution License
└── .gitignore                  # Environment variables (e.g., .env)
```

## 🚀 Getting Started

### Prerequisites
- Python 3.6+
- Jupyter Notebook
- Basic libraries: `csv` (built-in)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/Dextro111/apps-market-analysis-with-python.git
cd apps-market-analysis-with-python
```

2. (Optional) Create a virtual environment:
```bash
python -m venv .env
source .env/bin/activate  # On Windows: .env\Scripts\activate
```

3. Launch Jupyter Notebook:
```bash
jupyter notebook
```

4. Open `playstoreAnalysis.ipynb` and run the cells sequentially.

## 📝 Notebook Contents

### Core Functions

1. **`explore_data(dataset, start, end, rows_and_columns=False)`**
   - Display dataset subsets with optional row/column counts

2. **`english_chars(name)`**
   - Filter apps by English character content
   - Removes non-ASCII characters (threshold: >3 non-ASCII chars)

3. **`frequency_table(dataset, index)`**
   - Generate frequency tables with percentage distributions
   - Analyzes any column by index

4. **`display_table(dataset, index)`**
   - Sorted frequency table display in descending order

### Analysis Workflow

1. **Data Loading**: CSV parsing and initial exploration
2. **Cleaning**: Duplicate removal and malformed row detection
3. **Filtering**: English-only apps and free apps
4. **Analysis**: Category distribution and install rate calculations

## 📊 Dataset Details

### Columns Analyzed
- **App**: Application name
- **Category**: App classification (ART_AND_DESIGN, BUSINESS, GAME, etc.)
- **Rating**: User rating (1-5 scale)
- **Reviews**: Number of user reviews
- **Size**: App size in MB or variable
- **Installs**: Installation count range
- **Type**: Free or Paid
- **Price**: App cost
- **Content Rating**: Age/content classification
- **Last Updated**: Last modification date
- **Android Version**: Minimum required version

## 🔍 Key Findings

- **8,864** free English apps analyzed (after cleaning)
- **1,181** duplicate entries removed
- **33** distinct app categories
- Communication apps have the highest average install rate
- Family and Games categories dominate by quantity

## 🛠️ Technologies Used

- **Python 3.6+**
- **Jupyter Notebook**: Interactive analysis environment
- **CSV Module**: Data parsing

## 📄 License

This work is licensed under the **Creative Commons Attribution 3.0 Unported License**.

To view a copy of this license, visit: http://creativecommons.org/licenses/by/3.0/

**You are free to:**
- Share — copy and redistribute the material
- Adapt — remix, transform, and build upon the material for any purpose, even commercially

**Under the following terms:**
- Attribution — You must give appropriate credit, provide a link to the license, and indicate if changes were made

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report issues or suggest improvements
- Fork and submit pull requests
- Extend analysis to iOS data
- Add visualizations and statistical models

## 📧 Contact

For questions or feedback, please open an issue in this repository.

## 🙏 Acknowledgments

- Google Play Store Dataset
- Inspiration from data cleaning best practices
- Mobile app market research community

---

**Last Updated**: 2024  
**Status**: Active

# Automated Enterprise Value (EV) Analysis Tool

## 📈 Project Overview

The Automated Enterprise Value (EV) Analysis Tool is designed to streamline the process of calculating the Enterprise Value of multiple companies using reliable financial data from EDGAR (XBRL) and Yahoo Finance (yfinance). This tool aims to address the inherent complexity in identifying key financial components such as Cash and Debt, which vary widely across companies and do not follow a standardized pattern.

## 💡 Key Challenges Addressed

One of the main challenges in financial analysis is determining which financial statement items should be considered as Cash or Debt. Different companies may use distinct accounting terms or categorize financial elements differently in their filings. For instance:

- **Cash** could be listed as “Cash and Cash Equivalents,” “Short Term Investments,” or even more obscure terms.
- **Debt** may appear as “Long Term Debt,” “Notes Payable,” or under other specific labels.

The lack of a universal standard can lead to inconsistencies and errors in manual analysis. This tool tackles this issue by automating the classification of financial items, ensuring accurate and consistent EV calculations across various companies.

## 🚀 Features

- **Automated Data Collection**: Retrieves company filings (10-K and 10-Q) from EDGAR and financial data from Yahoo Finance.
- **Smart Classification System**: Automatically identifies relevant Cash and Debt items in financial statements using a combination of predefined rules and fallback strategies.
- **Data Correlation and Validation**: Cross-references XBRL data (considered highly reliable) with Yahoo Finance data to validate or override discrepancies.
- **Batch Processing**: Optimized for analyzing multiple companies simultaneously, significantly reducing the manual effort required.
- **Comprehensive Reporting**: Generates detailed financial reports, including EV, Market Cap, Cash, and Debt metrics, with export options to CSV and Excel.

## 📊 Technologies Used

- **Programming Language**: Python
- **Libraries**:
  - `yfinance`: For retrieving historical market data.
  - `pandas`: Data manipulation and analysis.
  - `matplotlib`: Visualization of financial metrics.
  - `edgar`: Access to EDGAR filings.
  - `logging`: Ensures detailed logs for debugging and transparency.

## 🧠 Research and Analysis Insights

The primary focus of this tool is to facilitate Research and Analysis by providing an automated method to collect and process financial data. It is particularly useful for analysts who need to evaluate the EV of multiple companies over different periods, offering a robust and scalable solution for financial modeling and decision-making.

## 🚦 How It Works

1. **Data Collection**
   - Retrieves company financials from EDGAR (10-K and 10-Q filings) and historical price data from Yahoo Finance.
2. **Processing & Classification**
   - Applies predefined rules to identify relevant financial items as Cash and Debt.
   - Uses a fallback system to handle unusual or company-specific accounting terms.
3. **Enterprise Value Calculation**
   - Computes the EV using the formula:
   
   \[
   EV = Market Cap + Debt - Cash
   \]

4. **Validation & Override System**
   - Automatically validates XBRL data against Yahoo Finance values.
   - Provides manual override options when discrepancies exceed a predefined threshold.
5. **Visualization & Export**
   - Generates charts to visualize the EV and its components over time.
   - Exports data to both CSV and Excel formats for further analysis.

## 📂 Sample Output

![EV Chart](outputs/sample_ev_chart.png)

## 🛠️ Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/enterprise-value-analysis.git
cd enterprise-value-analysis
```

### 2. Install the Required Packages
```bash
pip install -r requirements.txt
```

### 3. Run the Analysis
```bash
python scripts/data_collection.py
python scripts/calculate_ev.py
python scripts/visualization_export.py
```

### 4. View the Results
- Check the `outputs` folder for generated reports and charts.

## 📬 Contact

- **Name:** Ariel Oliveira
- **LinkedIn:** https://www.linkedin.com/in/arieloliveirasj/
- **Email:** arieloliveirasj@hotmail.com


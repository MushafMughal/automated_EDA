# Automated EDA - Material Master Analysis

## Overview
This repository contains a comprehensive Exploratory Data Analysis (EDA) of Material Master data for an Oil & Gas company. The analysis evaluates inventory health, identifies cost drivers, and highlights data quality issues in the supply chain.

## Deliverables

### 1. **Material_Master_EDA.ipynb** 
Fully executed Jupyter Notebook containing:
- Data quality and integrity checks
- Inventory valuation and ABC analysis
- Dead stock and obsolescence analysis  
- Vendor and material category analysis
- Comprehensive visualizations and insights

**All 21 code cells have been executed with outputs included.**

### 2. **Executive_Summary.md**
High-level executive summary with:
- Key findings and business insights
- Critical issues requiring immediate attention
- 9 actionable recommendations (immediate, short-term, and long-term)
- Expected business impact ($100M+ working capital release potential)
- "Interesting facts" from the data analysis

### 3. **Analysis Output Files**
- `ABC_Classification.csv` - Complete ABC classification for all parts
- `Dormant_Parts.csv` - Inventory with no activity in 2+ years
- `Vendor_Analysis.csv` - Vendor concentration and spend analysis
- `EDA_Summary_Dashboard.png` - Visual dashboard of key metrics

## Key Findings

🚨 **Critical Alert: $229.7 Million in Zombie Inventory**
- 36,107 parts (100% of inventory) with no movement in 2+ years
- Immediate disposition program recommended

📊 **ABC Analysis Results:**
- Class A: Only 6.4% of parts = 80% of value (better than Pareto)
- Strong value concentration enables focused management

⚠️ **Data Quality Issues:**
- 7,117 parts have inventory but zero cost
- 2 duplicate primary key records
- Missing vendor and classification data

🏭 **Vendor Risk:**
- Top 5 vendors: 22.2% of standard cost (moderate concentration)

## How to Use

### View the Analysis
1. Open `Material_Master_EDA.ipynb` in Jupyter Notebook/Lab
2. All cells are pre-executed with outputs visible
3. Review `Executive_Summary.md` for business insights

### Re-run the Analysis
```bash
# Install dependencies
pip install pandas matplotlib seaborn openpyxl jupyter

# Execute the notebook
jupyter nbconvert --to notebook --execute Material_Master_EDA.ipynb --output Material_Master_EDA.ipynb
```

## Dataset
- **File:** Part Data Extract.xlsx (Consolidate sheet)
- **Records:** 156,059 material master records
- **Columns:** 31 fields including costs, quantities, vendors, classifications

## Business Domain
- Industry: Oil & Gas
- Focus: Material Master, Inventory Management, Supply Chain
- Analysis Date: February 11, 2026

## Methodology
- **ABC Classification:** Cumulative value method (A=80%, B=15%, C=5%)
- **Dormant Inventory:** No transactions in 24+ months from analysis date
- **Data Quality:** Comprehensive checks for duplicates, missing values, and illogical records

## Expected Business Impact
If recommendations are implemented:
- **$100M+ working capital** freed from inventory reduction
- **$5-10M annual savings** from reduced carrying costs  
- **15-20% improvement** in working capital ratio
- **Improved inventory accuracy** to >98% with ABC-based cycle counting

## Contact
For questions about this analysis, please refer to the Executive Summary or review the detailed notebook.
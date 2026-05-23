#Decodelab Data Analytics — Project 1

#About
As part of my industrial training at DecodeLabs, this project 
represents the foundation phase of my Data Analytics journey. 
The focus was not on building dashboards or models — it was 
about getting the data right. Before any meaningful analysis 
can happen, the data has to be trustworthy. Raw datasets are 
often messy and dirty and this project was about transforming 
that noise into a clean reliable source of truth.


#The Dataset
A raw e-commerce orders dataset containing 1,200 records across 
14 columns — covering everything from order details and payment 
methods to shipping addresses and coupon usage.

#What I Did

**Phase 1 — Handling Missing Values**
Discovered 309 missing entries in the CouponCode column. Rather 
than deleting those rows and losing data, I filled them with 
'NO COUPON' to accurately reflect that those customers simply 
did not apply a discount code. All 1,200 records were preserved.

**Phase 2 — Removing Duplicates**
Ran a full audit on every row and OrderID in the dataset. 
Zero duplicates were found, confirming the dataset had no 
inflated or repeated records.

**Phase 3 — Standardizing Formats**
Verified and confirmed consistency across all columns including 
date formats, text casing and numeric precision. The dataset 
was already well structured in most areas and that was documented 
honestly rather than making unnecessary changes.


#Tools Used
- Python
- Pandas
- 
#How To Run
1. Clone this repository
2. Install pandas: `pip install pandas`
3. Run `explore.py` to inspect the raw dataset
4. Run `phase1_imputation.py`
5. Run `phase2_duplicates.py`
6. Run `phase3_formatting.py`
7. Cleaned file saved to `output/cleaned_data.csv`

#Outcome
1,200 records cleaned and prepared for analysis with zero 
data loss. The dataset is now production ready and meets 
the DecodeLabs verification standard of zero duplicate IDs 
and zero incorrectly formatted dates.

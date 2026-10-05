## 🗂️️ Subject Overview
1. **Paper 1:** Digital Image Processing (DIP) 
2. **Paper 2:** Data Warehousing & Data Mining (DWDM) 
3. **Paper 3:** Artificial Intelligence (AI)


# Data Warehouse and Data Mining (exam perpuse notes)


Q3- 4 Marks!!

# Question:- Data Cleaning & Binning Techniques
- Data Cleaning is the process of removing errors and noise from data to make it accurate and useful.
1. Binning
Binning is used to smooth noisy data by dividing data into small groups called bins.
Two common methods are:
# Equal-Width Binning:
Data range is divided into bins of equal size/range.
Example: 0–10, 10–20, 20–30.
# Equal-Frequency Binning:
Each bin contains approximately the same number of data values.

2. Smoothing by Bin Mean
Replace all values in a bin with the average (mean) of that bin.
Example: 10, 12, 14 → 12, 12, 12

3. Smoothing by Bin Median
Replace all values in a bin with the middle value (median).
Example: 10, 12, 20 → 12, 12, 12

4. Smoothing by Bin Boundaries
Replace each value with the nearest boundary value (minimum or maximum) of the bin.
Example: 10, 12, 14 → boundaries are 10 and 14; 12 is replaced by the nearest boundary.

Example: 
* Sorted data: 4, 8, 15, 21, 21, 24, 25, 28, 34
* Partition into bins of size 3:
> Bin 1: 4, 8, 15
> Bin 2: 21, 21, 24
> Bin 3: 25, 28, 34
* Smoothing by Bin Means:
> Bin 1 mean = (4+8+15)/3 = 9  ---> [9, 9, 9]
> Bin 2 mean = (21+21+24)/3 = 22 --->[22, 22, 22]
> Bin 3 mean = (25+28+34)/3 = 29 ---> [29, 29, 29]



# Q2-  Difference Between OLAP & OLTP 

# OLAP	
1. OLAP stands for Online Analytical Processing.	
2. Used for data analysis and decision-making.	
3. Works mainly with large amounts of historical data.
4. Queries are usually complex and analytical.	
5. Example: Analyzing yearly sales trends.	

# OLTP
1. OLTP stands for Online Transaction Processing.
2. Used for daily transactions and operations.
3. Works mainly with current/real-time data
4. Queries are usually simple and fast.
5. Example: ATM withdrawal, billing, or online order.


# Q3- 🟢 OLAP Operations & Data Cube Technology
OLAP is used to analyze data from different views using a data cube.
1. Roll-up
Combines detailed data into higher-level summary data.
Example: Daily sales → Monthly sales → Yearly sales.
2. Drill-down
Goes from summary data to more detailed data.
Example: Yearly sales → Monthly sales → Daily sales.
3. Slice
Selects one particular value from one dimension.
Example: Viewing only 2026 sales from all sales data.
4. Dice
Selects data using multiple conditions/dimensions.
Example: Viewing 2026 sales of laptops in Mumbai.
5. Pivot
Changes the view/orientation of data to see it differently.
Example: Changing a report from product-wise sales to region-wise sales.


# Q 4- Supervised Learning & unsupervised Learning 

# :- Supervised Learning 
- Supervised Learning learns from labeled data.
- The correct answer/output is already given in the training data.
- It is mainly used for classification and prediction.
- Example: Classifying emails as Spam or Not Spam.

# :- Unsupervised Learning
- Unsupervised Learning works with unlabeled data.
- There is no predefined answer/output given.
- It finds groups or patterns in the data.
- It is mainly used for clustering.
- Example: Grouping customers into different groups based on their buying habits.


# Q5- Data Integration & Redendancy Handling 
# 1. Data Integration — 4 Marks

- Definition: Data Integration means combining data from different sources into one common system.

1. Entity Identification: Identifying the same entity in different databases.
2. Data Value Conflicts: Resolving different formats or values for the same data.
3. Data Transformation: Converting data into a common format.
4. Data Consistency: Ensuring the combined data is accurate and consistent.


# 2. Redundancy Handling — 4 Marks

- Definition: Redundancy handling means identifying and removing duplicate or unnecessary data.

1. Duplicate Data: Same information may appear multiple times.
2. Correlation Test (χ²): Checks whether two categorical attributes are related.
3. Remove Redundancy: Unnecessary or repeated data is removed.
4. Benefit: Reduces storage and improves data accuracy.


# Q 6- Issues Regarding Classification & Prediction — 4 Marks
- Accuracy: The model should give correct predictions with minimum errors.
- Speed: The model should classify and predict results quickly.
- Robustness: The model should work properly even when data contains noise or errors.
- Scalability: The model should handle large amounts of data efficiently.
- Interpretability: The results of the model should be easy to understand and explain.
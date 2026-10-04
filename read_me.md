## 🗂️️ Subject Overview
1. **Paper 1:** Digital Image Processing (DIP) 
2. **Paper 2:** Data Warehousing & Data Mining (DWDM) 
3. **Paper 3:** Artificial Intelligence (AI)


# Data Warehouse and Data Mining (exam perpuse notes)


Q3- 4 Marks!!

# Data Cleaning & Binning Techniques
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
# # EA2_Data_Cleaning_and_Transformation

# 📦 Product Sales Dataset

## 📌 Project Overview

This dataset contains sample product information, including product IDs, product names, brand names, prices, quantities, categories, price ranges, and date-related attributes.

It can be used for practicing data analysis, data visualization, Excel, SQL, Python, and Power BI.


## 🎯 Project Objectives

● Handling Missing Values
● Correcting Inconsistent Data
● Removing Duplicates
● Splitting and Merging Data
● Number Formatting
● Conditional Formatting


## 🛠️ Tools and Technologies

This dataset can be used with:

- Microsoft Excel

  📂 Dataset Description
The dataset contains the following columns:

<img width="787" height="372" alt="image" src="https://github.com/user-attachments/assets/fb08c626-460e-44ec-a864-b0f3d64424aa" />

**1. Handling Missing Values:-**

•	Checking for missing values in the 'Price' column. Using **Isblank** function to fill 
blank column and **Average** function to find the average price of the column.

Formula Used:-

**=ROUND(IF(ISBLANK([@[Price ($)]]),AVERAGE([Price ($)]),[@[Price ($)]]),0)**

<img width="940" height="692" alt="image" src="https://github.com/user-attachments/assets/03cc29f5-a1cd-41af-9531-274f02e36de5" />

● If there are products with missing categories, I used **Isblank** function to fill the column and used **Pivot table** to find the count of the category and I choose top category **Electronics** to fill the blanks.

<img width="940" height="312" alt="image" src="https://github.com/user-attachments/assets/2690cb9e-8bc4-471f-95fe-69333d7b77d3" />

Formula Used:-

**=IF(ISBLANK([@Category]),"Electronics",[@Category])**

<img width="940" height="432" alt="image" src="https://github.com/user-attachments/assets/59b886c7-e12d-4f60-bd38-81fd04ad7e1b" />

**2. Correcting Inconsistent Data:-**

● Created product name standardization column and using function **Uppe**r to change first letter in the product name in **upper case**.

Formula Used:-

**=UPPER(LEFT(B13,1))&LOWER(MID(B13,2,LEN(B13)))**

<img width="940" height="496" alt="image" src="https://github.com/user-attachments/assets/75916db8-ec71-4b66-8809-86f0cef41a3b" />

● Using find and replace to find the misspelling and replace the correct spelling ,change the Electroni into Electronics.

<img width="940" height="344" alt="image" src="https://github.com/user-attachments/assets/599d1c52-c0cb-4789-9d25-5c34293bfa45" />

**3. Removing Duplicates:-**

● Identified the duplicate using **power query table** and click the remove duplicates to remove the duplicate rows in the product id Column.

<img width="940" height="263" alt="image" src="https://github.com/user-attachments/assets/17dc2ff9-850b-4dc7-bfd8-7f3d5a1d170d" />

**4. Splitting and Merging Data:-**

● Spliting the "Product ID" column into two separate columns for " Manufacturing Date"
and "Country Code” using **Textbefore** and **Textafter** functions.

Formula Used:-

**=TEXTBEFORE(A13,"-",2)**
**=TEXTAFTER(A13,"-",2)**

<img width="940" height="258" alt="image" src="https://github.com/user-attachments/assets/82944b35-f64c-4417-9179-65a6fe478dd5" />

● Merging the "Brand Name" and "Product Name" columns into one column named "Product Brand" using **CONCATENATE** function.

Formula Used:-

**=CONCATENATE([@[Product Name]]," ",[@[Brand Name]])**

<img width="940" height="241" alt="image" src="https://github.com/user-attachments/assets/655d5d13-0a8d-456e-b0f0-f7fc22ca310b" />

**5. Number Formatting:-**

● Formating the data type of the "Price" column into a currency format first selecting the price column and **click-->Home-->General-->Currency**

<img width="940" height="451" alt="image" src="https://github.com/user-attachments/assets/1e7baaa6-18f4-4727-96ed-fbbe3607fd91" />

● Formating the "Manufacturing Date" column to display dates in the "DD-MM-YYYY " format. But Year is missing in the dataset 

<img width="592" height="162" alt="image" src="https://github.com/user-attachments/assets/1fdcfee1-1cb1-4c80-a108-11eb7fd241bd" />

**6. Conditional Formatting:-**

● Applying data bar conditional formatting in the "Price" column.

<img width="940" height="454" alt="image" src="https://github.com/user-attachments/assets/bb2b4313-c97b-4344-aff7-c941e37d6c55" />

● Creating a custom rule for conditional formatting in the "Category" column to highlight cells where the category is "Electronics."

<img width="940" height="463" alt="image" src="https://github.com/user-attachments/assets/461781f7-b0d7-464e-bf8b-f9212bc0c537" />

 **6.Final Outputs:-**

<img width="1846" height="562" alt="image" src="https://github.com/user-attachments/assets/6bafbb56-fd83-4d2d-b872-22d7ee8ce334" />


**Key Learnings**
Through this project, I practiced:

statistical analysis using AVERAGE.
Mathematical and Aggregate functions.
Text functions.
Power Query using Remove duplicates.
Data imputation using ISBLANK in Numerical and Categorical.
Date and Time Functions.
Conditional Formating.


## 👤 Author

**Bhavani**

Aspiring Data Analyst | Excel | SQL | Python | Power BI

---

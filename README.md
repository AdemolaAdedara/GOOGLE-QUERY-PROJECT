### Google Query Project
---
### Overview
---
This project is designed to provide hands-on experience with Google Sheets' QUERY function, a powerful tool for data filtering, sorting, and aggregation. This repository contains practical data sets to help users learn how to harness the capabilities of the QUERY function for data analysis within Google Sheets.

----

### Table of Contents
---
- [Overview](#overview)

- [Features](#features)

- [Getting Started](#getting-started)
  
- [Usage](#usage)
  - [Example Queries](#example-queries)
  
---

### Features
---
- **Data Filtering**: Learn to filter data by various criteria, including dates, text, and numbers.

- **Data Aggregation**: Utilize functions like `SUM`, `COUNT`, `MAX`, `MIN`, and `AVG` within queries to perform data aggregation.

- **Sorting**: Sort results based on specified columns in either ascending or descending order.

- **Logical Operations**: Apply `AND`, `OR`, and `LIKE` operations to create complex conditions.

- **Data Transformation**: Transform data by combining columns or extracting subsets based on criteria.

---

### Getting Started
---
git clone https://github.com/Demmymoney/google-query-project.git

---

### Prerequisites
---
Make sure you have access to Google Sheets and a Google account to test the QUERY function

---

### Usage
---
In this section, you'll explain the pictures of the data set and Data Points extracted to demonstrate how to effectively use the QUERY function in Google Sheets.

---

#### Example Queries
---
1) ![Picture 1](https://github.com/Demmymoney/GOOGLE-QUERY-PROJECT/blob/main/GITHUB%201.png)
*This image shows the raw data used in the examples. Beside it are the first two Data Points extracted using the QUERY functions below:*

- **Example QUERY Function**:
  
- i) The Region, Sales_rep, and Item Data Point was extracted using the following Query function;

  ```excel
  = QUERY(A:H, "SELECT A, B, C", 1)

- ii) The Region, Year, and Sales Data Point was extracted using the following Query function;

  ```excel
  = QUERY(A:H, "SELECT A, F, H", 1)
---
2) ![Picture 1](https://github.com/Demmymoney/GOOGLE-QUERY-PROJECT/blob/main/GITHUB%202.png)
*This image shows the three Data Points extracted using the QUERY functions below:*

- **Second Example QUERY Function**:

- i) The Sales_rep who sold only "Pen" and "Binder" Data Point was extracted using the following Query function;

  ```excel
  =QUERY(A1:H44, "SELECT B,C WHERE C = 'Pen' OR C = 'Binder'", 1)

- ii) Only Sales_rep and item Data Point was extracted using the following Query function;

  ```excel
  =QUERY(A:H, "SELECT B,C ")

- iii) Only Sales_rep and Region Data Point was extracted using the following Query function;

  ```excel
  =QUERY(A:H, "SELECT A,B ")
---
3) ![Picture 1](https://github.com/Demmymoney/GOOGLE-QUERY-PROJECT/blob/main/GITHUB%203.png)
*This image shows the four Data Points extracted using the QUERY functions below:*

- **Third Example QUERY Function**:

- i) Only Items sold by "Richard" and "Matthew" Data point was extracted using the following Query function;

  ```excel
  =QUERY(A:H, "SELECT B,C WHERE B ='Richard' OR B= 'Matthew'", 1)
  
- ii) Region with Only Sales_rep "Richard" Data Point was extracted using the Query function;

  ```excel
  =QUERY(A:H, "SELECT A,B WHERE B = 'Richard' ",1)

- iii) Items sold in 2014 Data Point was extracted using Query function;

  ```excel
  =QUERY(A1:H44, "SELECT C,F,H WHERE F='2014'",1)

- iv) Sales made in 2015 Data Point was extracted using the Query function;

  ```excel
  =QUERY(A1:H44, "SELECT A,F,H WHERE F = '2015'", 1)
---
4) ![Picture 1](https://github.com/Demmymoney/GOOGLE-QUERY-PROJECT/blob/main/GITHUB%204.png)
*This image shows the four Data Points extracted using the QUERY functions below:*

- **Fourth Example QUERY Function**:

- i) Region where "Binder" and "Pen" were sold in 2014 Data Point was extracted using the Query function;

  ```excel
  =QUERY(A1:H44, "SELECT A, C, F WHERE (C = 'Binder' OR C = 'Pen') AND F = '2014' ", 1)

- ii) "East" Region sales in 2014 & 2015 Data Point was extracted using the Query function;

  ```excel
  =QUERY(A1:H,"SELECT A,F,H WHERE A = 'East' ",1)

- iii) Sales of "Binder" and "Pencil" in 2015 Data Point was extracted using the Query function;

  ```excel
  =QUERY(A:H, "SELECT C,F,H WHERE (C = 'Binder' OR C = 'Pencil') AND F = '2015'",1)

- iv) Sales in "Central" and "East" Region in 2014 Data Point was extracted using Query function;

  ```excel
  =QUERY(A:H, "SELECT A,F ,H WHERE ( A = 'Central' OR A = 'East') AND F = '2014'",1 )
---
5) ![Picture 1](https://github.com/Demmymoney/GOOGLE-QUERY-PROJECT/blob/main/GITHUB%205.png)
*This image shows the five Data Points extracted using the QUERY functions below:*

- **Fifth Example QUERY Function**:

- i) Sales in "Aug" and "Sep" in 2014 Data Point was extracted using Query function;

  ```excel
  =QUERY(A:H, "SELECT E, F, H WHERE (E = 'Aug' OR E = 'Sep') AND F = '2014'", 1)

- ii) Sales made by "Richard" in 2014 from highest to lowest order Data Point was extracted using the Query function;

  ```excel
  =QUERY(A:H,"SELECT B,H,F WHERE B = 'Richard' AND F = '2014' ORDER BY H DESC",1)

- iii) Item sold on the fourth day of the seventh and twelfth month in 2014 Data Point was extracted using Query function;

  ```excel
  =QUERY(A:H,"SELECT C, D, E, F WHERE D LIKE '%_04%' AND (E = 'Jul' OR E = 'Dec') AND F = '2014'",1)

- iv) Region where the Sales_rep name starts with the letter "R" Data Point was extracted using the Query function;

  ```excel
  =QUERY(A:H, "SELECT A,B WHERE B LIKE 'R%'",1)
 
- v) Item sold by Sales_rep with "an" in their name Data Point was extracted using the Query function;

  ```excel
  =QUERY(A:H,"SELECT B,C WHERE B LIKE '%an%'",1)




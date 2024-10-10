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
  
- [Project Structure](#project-structure)

### Features
---
- **Data Filtering**: Learn to filter data by various criteria, including dates, text, and numbers.

- **Data Aggregation**: Utilize functions like `SUM`, `COUNT`, `MAX`, `MIN`, and `AVG` within queries to perform data aggregation.

- **Sorting**: Sort results based on specified columns in either ascending or descending order.

- **Logical Operations**: Apply `AND`, `OR`, and `LIKE` operations to create complex conditions.

- **Data Transformation**: Transform data by combining columns or extracting subsets based on criteria.

### Getting Started
---
git clone https://github.com/Demmymoney/google-query-project.git

## Prerequisites
---
Make sure you have access to Google Sheets and a Google account to test the QUERY function

### Usage
---
In this section, you'll explain the pictures of the examples to demonstrate how to effectively use the QUERY function in Google Sheets.

### Example Queries

1) ![Picture 1](https://github.com/Demmymoney/GOOGLE-QUERY-PROJECT/blob/main/GITHUB%201.png)
*This image shows the raw data used in the examples. Beside it are the first two data points extracted using the QUERY functions:*

- **Example QUERY Function**:
  
- i) The region, sales_rep, and items were extracted using the following Query function:

  ```excel
  = QUERY(A:H, "SELECT A, B, C", 1)

- ii) The region, year, and sales were extracted using the following Query function

  ```excel
  = QUERY(A:H, "SELECT A, F, H", 1)


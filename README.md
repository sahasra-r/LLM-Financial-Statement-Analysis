# LLM-Assisted Financial Statement Analysis Tool

An intelligent financial analysis system that extracts financial information from annual reports, validates and normalizes the extracted data, calculates financial ratios programmatically, performs trend analysis, and uses a Large Language Model (LLM) to generate clear and grounded explanations.

---

## 📌 Project Overview

Financial statements and annual reports contain large amounts of structured and unstructured information, making manual analysis time-consuming and difficult, especially for students, analysts, and users without a strong financial background.

The **LLM-Assisted Financial Statement Analysis Tool** automates the major stages of financial statement analysis.

The system accepts an annual financial report in PDF format, extracts relevant financial information, converts it into a structured format, validates the extracted values, calculates important financial ratios, performs year-over-year analysis, and provides an understandable explanation using an LLM.

A key design principle of this project is that the **LLM does not independently calculate financial ratios or invent financial values**. Financial calculations are performed programmatically, while the LLM is used to explain verified results.

---

## 🎯 Objectives

The main objectives of this project are:

- Extract financial information from annual reports and financial PDFs.
- Convert extracted information into a structured financial data format.
- Normalize financial values and terminology.
- Validate extracted data before performing calculations.
- Calculate important financial ratios programmatically.
- Perform year-over-year and trend analysis.
- Identify potential financial trends and red flags.
- Generate simple, understandable explanations using an LLM.
- Provide a user-friendly interface for viewing financial analysis.
- Maintain traceability between extracted data, calculations, and generated explanations.

---

## 🚀 Key Features

### 📄 PDF Financial Data Extraction
Extracts relevant financial information from annual reports and financial documents.

### 🧹 Data Normalization
Converts extracted values into a consistent and structured format suitable for analysis.

### ✅ Data Validation
Checks whether required financial information is available and valid before calculations are performed.

### 📊 Financial Ratio Calculation
The system programmatically calculates important financial ratios such as:

- Current Ratio
- Return on Equity (ROE)
- Debt-to-Equity Ratio

Additional financial indicators can be incorporated into the analysis framework.

### 📈 Trend Analysis
Compares financial values across multiple years to identify:

- Growth
- Decline
- Stable performance
- Significant changes
- Potential financial concerns

### 🤖 LLM-Based Financial Explanation
The LLM converts verified financial results into human-readable explanations.

Instead of asking the LLM to perform calculations, the system provides the LLM with verified values and calculated results.

### 🖥️ Interactive Interface
A user-friendly interface can be used to upload financial documents and display extracted information, calculated ratios, trends, and explanations.

---

## 🏗️ System Architecture

The overall workflow of the system is:

```text
                Financial Report PDF
                         │
                         ▼
                ┌─────────────────┐
                │ PDF Extraction  │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │  Normalization  │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │   Validation    │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │ Ratio Calculator│
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │ Trend Analysis  │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │ Verified Results│
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │       LLM       │
                │  Interpretation │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │ Analysis Output │
                └─────────────────┘

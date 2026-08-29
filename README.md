# CyberRisk_FinalProject_TCPRO2026
Mobile app built with MIT App Inventor for the Tecnolochicas PRO final project. It analyzes CVE databases using regression models to predict CVSS risk based on attack vectors and complexity, featuring real-time AI integration for threat assessment.

# CVE Database Explorer (CyberRisk)
**Mobile application for predictive cybersecurity vulnerability analysis**

Description • Features • Installation • Usage • Models • Structure • Technologies

## Description
**CVE Database Explorer** is a specialized mobile application for cybersecurity risk assessment, developed in MIT App Inventor as a final project for Tecnolochicas PRO. The application processes historical vulnerability data, implementing linear and polynomial regression models to predict the severity of threats (CVSS scores) based on attack vectors and complexity.

Connected directly to Google Sheets, it features interactive data visualization, an integrated data cleaning module, advanced mathematical modeling, and an AI-driven predictive engine.

The dataset is based on public standardized cybersecurity records (CISA 2022) that underwent a rigorous preprocessing and sanitization protocol. All application design and programming are the exclusive property of the Author. All rights reserved.

## Features 

### Visualization and Analysis
*   Real-time connection with Google Sheets.
*   **Interactive Charts:**
    *   Vector (Access Type) vs CVSS Score.
    *   Attack Complexity vs CVSS Score.
*   **Data Depuration:** Interactive module to filter null values, clean empty rows, and transform categorical variables into ordinal metrics.

### Implemented Mathematical Models
*   **Linear Regression (Vector Penalty)**
    *   Y = MX + B
    *   Calculates the constant growth of risk based on remote accessibility (Local -> Network).
*   **Polynomial/Exponential Regression (Threat Scaling)**
    *   Adapts to non-linear risk spikes associated with varying levels of exploit complexity.
    *   Calculates accurate trendlines while mitigating standard logarithmic overflow errors (NaN).
*   **AI Predictive Engine**
    *   Concatenates live application variables (Correlation Coefficient R, Slope M, Y-Intercept B).
    *   Predicts future vulnerability impact and provides dynamic mitigation strategies for IT infrastructure.

## Installation

**Prerequisites**
*   Google Account with access to Google Sheets.
*   MIT App Inventor 2.0+ environment.
*   Android device or MIT AI2 Companion app for testing.

## Usage
1.  Import the provided `.aia` file into your MIT App Inventor account.
2.  Update the Web component URL to point to your specific Google Sheets deployment script.
3.  Load the application on your device.
4.  Navigate through the bottom menu: **Show Data** -> **Clean Data** -> **Draw Lines of Best Fit** -> **AI Analysis**.

## Technologies
*   **Frontend & Logic:** MIT App Inventor (Block-based programming)
*   **Database:** Google Sheets / Kaggle Datasets
*   **AI Integration:** Generative AI Chatbot component via API
*   **Data Preprocessing:** Categorical-to-Ordinal mapping algorithms

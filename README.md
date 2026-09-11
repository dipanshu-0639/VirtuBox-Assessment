# Customer 360 --- Business Analysis Assessment

## Overview

This project analyzes a large Customer 360 / order-level dataset to
understand order performance and identify practical opportunities for
business management.

The assessment covers data selection, cleaning, exploratory analysis,
business insights, recommendations, dashboard development, and
responsible use of AI.

## Dataset

**Dataset:** Customer 360\
**Source:** Kaggle --- Vinay Kandimalla\
**URL:** https://www.kaggle.com/datasets/vinaykandimalla/customer-360

The analysis uses **300,000 order records** after processing.

## Assessment Structure

### Q1 --- Dataset Selection

A large publicly available Customer 360 dataset was selected because it
contains 300,000 records and provides enough data for meaningful
business analysis.

The dataset contains order-related information that can be used to study
order status, payment methods, order values, products, and trends over
time.

### Q2 --- Business Problem and Analysis Questions

The main objective was to understand overall order performance and
identify areas where the business could reduce unsuccessful orders and
improve customer/order outcomes.

The analysis focuses on questions such as:

-   How well are orders performing overall?
-   What proportion of orders are successful, failed, or refunded?
-   Does payment method appear to affect order success?
-   Which products generate the highest successful order value?
-   How does order activity change over time?

Hypotheses were developed around order success and payment/product
performance and were tested using the processed dataset.

### Q3 --- Data Processing

The raw data was processed using Python, Pandas, NumPy, Matplotlib,
Seaborn, and Google Colab.

Main cleaning activities included:

-   Checking the dataset structure and data types.
-   Handling inconsistent category values.
-   Standardizing **Order Status** values.
-   Standardizing **Payment Method** values.
-   Checking for duplicate or problematic records.
-   Checking date fields and identifying missing/invalid dates.
-   Preparing the cleaned dataset for analysis and dashboard creation.

The cleaning was necessary because inconsistent values such as different
spellings or shortened versions of the same category could otherwise be
counted as separate groups and lead to incorrect business conclusions.

### Q4 --- Exploratory and Descriptive Analysis

The processed dataset was analyzed using summary statistics and visual
comparisons.

Key areas examined included:

-   Overall order volume.
-   Successful, failed, and refunded orders.
-   Success rate by payment method.
-   Distribution of order-value categories.
-   Successful order value by product.
-   Monthly order activity.

The analysis was focused on findings that could be useful for management
rather than creating charts only for presentation purposes.

### Q5 --- Surprising / Unexpected Result

One important unexpected result was that the success rates across
payment methods were very similar.

Initially, it was reasonable to expect that some payment methods might
perform noticeably better or worse than others. After standardizing the
payment-method categories and comparing success rates, the differences
were relatively small.

This suggests that payment method alone may not explain most
unsuccessful orders. Further analysis would be required to identify the
operational or order-level factors behind failures and refunds.

### Q6 --- Data Quality, Limitations and Risks

Important data-quality and analytical considerations included:

1.  **Inconsistent category labels**\
    Different labels represented the same payment methods or order
    statuses. These were standardized during processing.

2.  **Missing or invalid dates**\
    Some records did not have usable order dates. Therefore, time-based
    analysis does not necessarily represent every record.

3.  **Descriptive analysis cannot prove causation**\
    The analysis identifies patterns and relationships, but it cannot
    safely prove that one variable directly caused an order to succeed
    or fail.

A conclusion that cannot safely be made is that a particular payment
method is the direct cause of failed orders.

### Q7 --- Management Recommendations

The main recommendations are:

1.  **Investigate failed and refunded orders**\
    Management should review the reasons behind unsuccessful orders and
    identify avoidable sources of order loss.

2.  **Prioritize high-performing products**\
    Products generating strong successful order value should receive
    appropriate attention in inventory and promotional planning.

3.  **Monitor order-performance KPIs regularly**\
    Management should track success, failure, and refund rates over time
    so that changes in performance can be identified early.

The recommendations are intended to be practical and measurable rather
than purely descriptive.

## Q8 --- Looker Studio Dashboard and Management Presentation

An interactive Looker Studio dashboard was created for a non-technical
management audience.

### Dashboard KPIs

-   Total Orders: **300,000**
-   Successful Orders: **221,280**
-   Success Rate: **73.76%**
-   Average Order Value: **45,455.18**

### Major Visualizations

-   Order Status Distribution
-   Success Rate by Payment Method
-   Order Value Distribution
-   Top 10 Products by Successful Order Value
-   Monthly Order Trend

### Interactive Filters

-   Order Status
-   Payment Method
-   Product
-   Date Range

The dashboard is designed to help management quickly understand order
performance and explore specific segments without working directly with
the raw dataset.

A separate management presentation summarizes the business problem,
methodology, key findings, deep-dive insight, recommendations, expected
business impact, limitations, and next steps.

## Q9 / Presentation Materials

The assessment includes a short senior-management presentation covering:

1.  Business Problem
2.  Data & Methodology
3.  Key Findings
4.  Deep-Dive Insight
5.  Recommendations
6.  Expected Business Impact
7.  Limitations & Next Steps

The presentation avoids unnecessary technical terminology and focuses on
business implications and decisions.

## Q10 --- How AI Was Used

ChatGPT was used as a support tool during the assessment.

It was mainly used for:

-   Guidance on data cleaning.
-   Analysis ideas.
-   Python/Google Sheets assistance.
-   Looker Studio setup guidance.
-   Improving the presentation of the analysis.

For example, AI helped identify inconsistent values in **Order Status**
and **Payment Method** and suggested how they could be standardized.

The suggested changes were checked against the actual Google Sheet data.
The dashboard was then refreshed to confirm that the cleaned categories
and calculated results behaved as expected.

## Tools Used

-   **Python**
-   **Pandas**
-   **NumPy**
-   **Matplotlib**
-   **Seaborn**
-   **Google Colab**
-   **Google Sheets**
-   **Looker Studio**
-   **ChatGPT** for limited analytical and technical assistance

## Final Deliverables

The assessment deliverables include:

-   Raw/selected dataset
-   Processed dataset
-   Q1 --- Dataset Selection
-   Q2 --- Business Problem, Questions and Hypotheses
-   Q3 --- Data Processing Explanation
-   Q4 --- Business Insights
-   Q5 --- Unexpected Result
-   Q6 --- Data Quality and Limitations
-   Q7 --- Management Recommendations
-   Q8 --- Looker Studio Dashboard and Management Presentation
-   Q10 --- How I Used AI
-   This README file

## Key Takeaway

The analysis shows a generally strong order-success rate, while failed
and refunded orders still represent an area worth investigating.
Payment-method success rates are relatively similar, so management
should avoid assuming that one payment method is responsible for
unsuccessful orders without additional evidence.

The next stage of analysis should focus on the reasons for
failed/refunded orders and other order-level factors that may explain
performance differences.

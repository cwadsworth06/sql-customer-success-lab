# SQL Customer Success Lab

This repository documents my hands-on SQL learning through practical Customer Success, SaaS, and account management scenarios.

## Purpose

I created this project to strengthen my SQL and data analysis skills in ways that connect directly to my professional background in Customer Success, implementation, account management, and SaaS.

Rather than focusing only on generic tutorial exercises, I am using SQL to explore questions that Customer Success and technical teams regularly encounter, including customer health, adoption, renewals, support activity, revenue, and expansion opportunities.

## Skills I Am Building

* Writing SQL queries
* Filtering and sorting data
* Using aggregate functions
* Grouping and summarizing data
* Working with multiple tables
* Using JOINs
* Analyzing customer and account data
* Identifying trends and risk signals
* Translating business questions into data queries

## Repository Structure

### 01-select-filtering

Basic SQL queries using:

* SELECT
* WHERE
* DISTINCT
* ORDER BY
* AND / OR
* IN
* BETWEEN
* LIKE

### 02-aggregations

Analysis using:

* COUNT
* SUM
* AVG
* MIN
* MAX
* GROUP BY
* HAVING

### 03-joins

Queries that combine customer, product, support, and renewal data using:

* INNER JOIN
* LEFT JOIN
* Multiple-table queries

### 04-customer-health-project

A practical SaaS Customer Success analysis project focused on questions such as:

* Which customers have upcoming renewals?
* Which accounts show declining product adoption?
* Which high-value customers may be at risk?
* Which customers have high support activity?
* Which accounts may represent expansion opportunities?
* How does customer health differ by segment?
* Which CSMs manage the largest ARR portfolios?

## Example Business Question

**Question:** Which enterprise customers have more than $100,000 in ARR and low product usage?

```sql
SELECT
    customer_name,
    arr,
    usage_score
FROM customers
WHERE segment = 'Enterprise'
    AND arr > 100000
    AND usage_score < 50
ORDER BY arr DESC;
```

This type of query could help a Customer Success team identify high-value accounts that may require additional adoption support or proactive risk mitigation.

## Learning Approach

My goal is to learn SQL through hands-on practice rather than passive coursework alone. I am combining structured SQL lessons with practical exercises based on realistic SaaS and Customer Success scenarios.

As I progress, this repository will include increasingly complex queries and a complete Customer Success data analysis project.

## Current Focus

I am currently working on SQL fundamentals, including querying, filtering, sorting, and aggregating data.

Future topics will include JOINs, CASE statements, subqueries, common table expressions, and more advanced customer data analysis.

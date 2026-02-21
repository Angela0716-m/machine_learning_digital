# Behavioral Learning Analytics & Engagement Prediction System

## Project Overview

This project develops a **Behavioral Learning Analytics Framework** that analyzes learner activity within a Learning Management System (LMS) to measure engagement, estimate confidence growth, and detect retention risk.

The system works with a small cohort of **50 users**, therefore the goal is not large-scale AI prediction, but rather interpretable analytics and behavioral modeling.

Instead of surveys, the system uses **real behavioral data** such as lesson activity and quiz performance to understand learning progress.

---

## Business Problem

The platform currently cannot objectively determine:

* Whether learners are improving over time
* Which learners are at risk of dropping out
* Whether engagement reflects actual learning
* How early behavior predicts long-term success

Organizations need a reliable way to monitor learning effectiveness using only platform usage data.

---

## Project Objective

Develop a behavioral analytics system that:

1. Tracks weekly learner engagement
2. Estimates confidence growth using activity patterns
3. Predicts early learner success
4. Detects churn risk
5. Validates analytics reliability
6. Generates weekly KPI reports

---

## Machine Learning & Analytics Tasks

### 1. Confidence Growth Modeling

Estimate learner confidence using behavioral indicators:

* Module completion rate
* Quiz performance
* Session frequency
* Learning consistency

A calculated confidence score is later validated using regression modeling.

---

### 2. Early Success Prediction

Predict whether a learner will successfully progress using first-week behavior.

Model Type:

* Logistic Regression
* Decision Tree (shallow)

---

### 3. Engagement Pattern Clustering

Group learners into behavioral categories:

* Highly engaged learners
* Moderate learners
* At-risk learners

Model Type:

* K-Means Clustering

---

### 4. Churn Risk Detection

Identify learners likely to stop using the platform based on inactivity patterns.

Model Type:

* Binary Classification

---

### 5. Analytics Validation

Detect unreliable learning signals such as:

* Rapid unrealistic completions
* Quiz score inconsistencies
* Suspicious activity behavior

Model Type:

* Isolation Forest
* Statistical anomaly detection

---

## Dataset Description

### Source

Learning Management System (LMS) activity database.

### Tables Used

* Users
* Courses
* Modules
* Lesson Activity Logs
* Quiz Attempts

Survey tables were intentionally excluded to ensure predictions rely only on behavioral data.

---

## Methodology

Because the dataset contains only 50 users, the project applies **longitudinal feature engineering**.

Instead of one row per user, data is transformed into weekly behavioral snapshots:

| user | week | sessions | modules_completed | avg_quiz | inactivity_days | confidence_score |
| ---- | ---- | -------- | ----------------- | -------- | --------------- | ---------------- |

This increases modeling reliability and reflects real learning progression.

---

## Machine Learning Lifecycle

1. Problem Definition
2. Data Cleaning (Python & Pandas)
3. Feature Engineering (Weekly behavioral aggregation)
4. Exploratory Data Analysis
5. Behavioral Modeling
6. Validation & Interpretation
7. KPI Dashboard Reporting

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* SQL
* Power BI / Visualization

---

## Expected Outcomes

The system will allow stakeholders to:

* Monitor learner progress weekly
* Detect struggling learners early
* Understand engagement behavior
* Improve course effectiveness
* Make data-driven training decisions

---

## Key Insight

This project demonstrates that meaningful learning analytics can be built even with small datasets by focusing on behavioral trends rather than complex AI models.

---

## Author

Behavioral Learning Analytics Project
Data Analytics & Machine Learning Portfolio Project

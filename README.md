# Subscription Conversion Rate Investigation

This project investigates the impact of a language-related issue on subscription conversions during a marketing campaign. The primary goal was to calculate how many subscriptions were lost when only English ads were served after January 11, 2018, while other languages (Spanish, Arabic, and German) were discontinued.

---

## 1. Data Description

The dataset `marketing.csv` contains the following columns:

- **user id**: Unique identifier for each user.
- **date served**: The date the ad was served to the user.
- **marketing channel**: The channel through which the ad was delivered.
- **variant**: A/B test variant shown to the user.
- **converted**: Boolean indicating whether the user subscribed after seeing the ad.
- **language displayed**: The language used to display the ad.
- **language preferred**: The user's preferred language.
- **age group**: The user's age group.
- **date subscribed**: The date the user subscribed, if they converted.
- **date canceled**: The date the user canceled their subscription, if applicable.
- **subscribing channel**: The channel through which the user subscribed.
- **is retained**: Boolean indicating whether the user retained their subscription over time.

---

## 2. Project Steps

The project was conducted in multiple steps, and the analysis is included in the notebook `conversion_rate_project.ipynb`:

### **Step 1: Required Libraries**

The necessary Python libraries used for this project include:

- `pandas`: For data manipulation and analysis.
- `numpy`: For numerical operations.
- `matplotlib`: For creating visualizations.
- `seaborn`: For enhanced data visualization.

### **Step 2: Conversion Rate Calculation**

- Calculated the total conversion rate and created a function to compute conversion rates for different groupings.

### **Step 3: Conversion Rate by Language**

- Computed conversion rates for each displayed language and visualized the differences using pie charts.

### **Step 4: Daily Conversion Rate Visualization**

- Visualized daily conversion rate trends over time using line plots.

### **Step 5: Conversion Rate Visualization Across Different Columns**

- Displayed conversion rates across multiple key dimensions such as marketing channel and language preferences using subplots.

### **Step 6: Daily Conversion Rate by Marketing Channel**

- Calculated and visualized the daily conversion rates for each marketing channel in separate subplots.

### **Step 7: Daily Conversion Rate by Language Displayed**

- Identified when specific languages stopped being offered and visualized their daily conversion rates with clear stop dates marked.

### **Step 8: Investigation: Impact of Language on Lost Subscriptions**

- Investigated how many subscriptions were lost due to the language issue and quantified the impact.

---

## 3. Conclusion

In this project, we found that discontinuing ads in Spanish, Arabic, and German before January 12, 2018, had a significant negative impact on conversions. After January 11, 2018, only English ads were served, resulting in approximately **38 lost subscriptions** during the period from January 11 to January 31, 2018. This analysis underscores the importance of offering localized content to maintain engagement and conversions across different language groups.

---

## 4. Project Files

The following files are used in this project:

- **`conversion_rate_project.ipynb`**: The main Jupyter notebook that contains the full analysis, including data processing, conversion rate calculations, and final conclusions.
- **`marketing.csv`**: The dataset used in this project, containing details about users, ads, and their interactions (conversion or non-conversion).

---

## 5. Requirements

To run this project, the following Python packages are required:

- `pandas`: For data manipulation and analysis.
- `numpy`: For numerical operations.
- `matplotlib`: For creating visualizations.
- `seaborn`: For enhanced data visualization.
- `jupyter`: For running the Jupyter notebook.

### Install the required libraries using the following command:

```bash
pip install pandas numpy matplotlib seaborn jupyter

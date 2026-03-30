# HR Dashboard w/ Tableau

![HR Dashboard Overview](/HR_Dashboard_Project/icons_&_images/Overview_1.png)

[🌐 **View Interactive Dashboard on Tableau Public**](https://public.tableau.com/app/profile/vladimir.vukoji.i./viz/HRDashboard_17729919518010/HRSummary)

## Introduction

This project was built to provide **HR Managers and People Analytics teams** with a clear, interactive view of workforce data. Using a synthetic dataset of **8,950 employee records**, this Tableau project delivers two dedicated dashboards — a **Summary View** covering workforce overview, demographics, and income analysis, and a detailed **Employee Records View** for in-depth individual analysis — enabling HR professionals to monitor hiring trends, workforce composition, salary patterns, and employee performance at a glance.

### Dashboard File

You can find the Tableau workbook file here: [`HR Dashboard.twbx`](HR%20Dashboard.twbx).

## Data Sources

The project uses a single synthetic dataset organized in the `dataset/` folder:

```
dataset/
├── HumanResources.csv   ← generated employee records (8,950 rows)
└── generate_data.py     ← Python script used to generate the dataset
```

The dataset was generated using a Python script (`dataset/generate_data.py`) that creates 8,950 realistic HR records with the help of ChatGPT-assisted prompts.

| Attribute | Description |
|-----------|-------------|
| **Employee ID** | Unique identifier for each employee |
| **First Name / Last Name** | Employee name |
| **Gender** | 46% Female, 54% Male probability |
| **State & City** | Selected from a predefined list of locations |
| **Hire Date** | 2015–2024 with custom year probabilities |
| **Department** | Assigned with specified probabilities |
| **Job Title** | Based on department with specific probabilities |
| **Education Level** | Derived from job title mapping |
| **Performance Rating** | Excellent, Good, Satisfactory, Needs Improvement |
| **Overtime** | 30% Yes, 70% No |
| **Salary** | Based on department and job title ranges |
| **Birth Date** | Based on age group distribution and job title requirements |
| **Termination Date** | 11.2% of employees; at least 6 months after hire date |
| **Adjusted Salary** | Calculated using gender, education level, and age multipliers |

## Assets

The [`icons_&_images/`](icons_&_images/) folder contains custom icons, background images, and dashboard screenshots used throughout the project to deliver a polished, app-like user experience — including navigation icons for switching between the Summary and Employee Records views, filter toggle icons, and branded backgrounds.

## Skills Showcased

This project demonstrates a broad range of Tableau and data skills:

-   **🎨 Dashboard Design & UX:** Designed clean, professional layouts with custom background images and intuitive navigation icons for switching between the Summary and Employee Records views.
-   **⚙️ Data Preparation:** Built the dataset using a Python script with ChatGPT-assisted prompts, generating 8,950 realistic synthetic employee records with controlled probability distributions.
-   **🧮 Calculated Fields:** Created custom calculations for employee status (active vs. terminated), age group bucketing, and salary adjustments based on gender, education, and age multipliers.
-   **📊 KPI Cards:** Built summary KPI cards showing total hired, active, and terminated employee counts at a glance.
-   **📈 Bar Charts & Trend Analysis:** Visualized hiring and termination trends over the years with bar and line charts to reveal workforce growth patterns.
-   **🗺️ Map Visualization:** Displayed employee distribution by state and city using Tableau's mapping capabilities.
-   **👥 Demographic Analysis:** Analyzed gender ratio, age group distributions, and education level breakdowns to understand workforce composition.
-   **📉 Correlation Analysis:** Presented the correlation between employees' educational backgrounds and their performance ratings.
-   **💰 Income Analysis:** Compared salaries across education levels and genders, and explored the age-salary correlation within each department.
-   **🎚️ Interactive Filters & Parameters:** Enabled dynamic filtering across all dimensions so users can drill into any workforce segment.
-   **📋 Employee Records Table:** Built a fully filterable employee records view listing name, department, position, gender, age, education, and salary.
-   **🖱️ Custom Navigation Icons & Dashboard Switching:** Used icon-based buttons to seamlessly navigate between the Summary and Employee Records dashboards.

---

## Dashboard Overview

*This project is split into two dedicated dashboards to provide focused, role-specific insights.*

### Dashboard 1: Summary View

The Summary View is organized into three tabs: **Overview**, **Demographics**, and **Income Analysis**.

**Overview Tab**

The Overview tab gives HR managers an immediate snapshot of the entire workforce:

- **KPI Cards** display the total number of hired employees, active employees, and terminated employees.
- A **trend chart** visualizes the total number of employees hired and terminated across each year (2015–2024).
- A **breakdown chart** presents total employees by department and job title.
- A **HQ vs. Branch comparison** compares total employees between New York headquarters and all other branch locations.
- A **geographic distribution** chart shows employees by city and state.

![HR Dashboard Overview 1](/HR_Dashboard_Project/icons_&_images/Overview_1.png)

![HR Dashboard Overview 2](/HR_Dashboard_Project/icons_&_images/Overview_2.png)

**Demographics Tab**

The Demographics tab digs into the makeup of the workforce:

- A **gender ratio** visualization shows the split between male and female employees.
- **Age group and education level distributions** reveal how employees are spread across different life stages and qualification levels.
- An **education vs. performance correlation** chart presents how educational backgrounds relate to performance ratings, helping to identify potential talent development patterns.

**Income Analysis Tab**

The Income Analysis tab surfaces compensation patterns and potential disparities:

- A **salary by education and gender** comparison highlights any discrepancies or patterns across qualification levels and genders.
- An **age-salary correlation** chart explores how compensation relates to employee age within each department.

### Dashboard 2: Employee Records View

The Employee Records View provides a comprehensive, filterable list of all employees in the organization. Each row includes key attributes such as name, department, position, gender, age, education level, and salary. Users can filter the list by any available column to quickly locate specific employees or explore workforce segments.

![HR Dashboard Details 1](/HR_Dashboard_Project/icons_&_images/Details_1.png)

![HR Dashboard Details 2](/HR_Dashboard_Project/icons_&_images/Details_2.png)

---

## Data Generation

The dataset was generated using the Python script at `dataset/generate_data.py`. The script uses ChatGPT-assisted prompts to define realistic probability distributions for each attribute, producing 8,950 synthetic HR records that closely mirror real-world workforce data patterns.

Key design decisions in the data generation process include:

- **Hire dates** are distributed across 2015–2024 using custom year probabilities to simulate realistic hiring waves.
- **Departments and job titles** are assigned using conditional probabilities to reflect typical organizational hierarchies.
- **Termination dates** affect 11.2% of employees and are always set at least 6 months after the hire date to simulate realistic tenure before departure.
- **Salary values** are based on department and job title ranges, then adjusted using multipliers for gender, education level, and age to introduce realistic variation.
- **Birth dates** are generated based on age group distributions appropriate for each job title, ensuring demographic realism.

The final dataset is saved as `dataset/HumanResources.csv` and loaded directly into the Tableau workbook.

---

## Conclusion

This Tableau project demonstrates how interactive dashboards can transform raw HR data into a powerful workforce intelligence tool. By separating the high-level summary from the detailed employee records into two dedicated views, HR managers can quickly switch between strategic insights and individual employee analysis — whether it's monitoring hiring trends, identifying demographic imbalances, spotting salary disparities, or reviewing individual employee profiles.

[🌐 **View Interactive Dashboard on Tableau Public →**](https://public.tableau.com/app/profile/vladimir.vukoji.i./viz/HRDashboard_17729919518010/HRSummary)

---

## 🙏 Acknowledgments

This project is part of the comprehensive Tableau course by **DataWithBaraa**. Special thanks to Baraa for creating excellent educational content on data analytics and Tableau!

**Connect with DataWithBaraa:**
- 🎥 [YouTube Channel](https://www.youtube.com/@DataWithBaraa)
- 🌐 [Website](https://www.datawithbaraa.com/)
- 💻 [GitHub](https://github.com/DataWithBaraa)

---

# Rafli Alfiansyah Portfolio
***


## [Project 1: An Investigation into Goal-Scoring Trends in International Soccer](https://github.com/Rafli-Alfiansyah/Hypothesis-Testing-with-Men-and-Women-Soccer-Matches)

A statistical analysis to validate the hypothesis that more goals are scored in women's FIFA World Cup matches than in men's, using data from 2002 onwards.

### **Analysis & Findings**

* **Dataset**: A filtered dataset of **200 women's** and **384 men's** official FIFA World Cup matches played since January 1, 2002.
* **Statistical Method**: A **Mann-Whitney U test** was used to compare the goal distributions between the two groups, with a significance level ($\alpha$) of **0.10**.
* **Result**: The test yielded a **p-value of ~0.0051**.

### **Conclusion**

Since the p-value (0.0051) is significantly less than $\alpha$ (0.10), the null hypothesis is **rejected**. The data provides strong statistical evidence that, in the modern era, **more goals are scored in women's World Cup matches than in men's**. ⚽

**Tool Used**: Python
***


## [Project 2: SAT Performance Analysis in New York City Public Schools](https://github.com/Rafli-Alfiansyah/Exploring-NYC-Public-School-Test-Result-Scores)

This project analyzes SAT performance data (`schools.csv`) from NYC public high schools to identify top-performing institutions and explore performance variations across the city's boroughs. 🎓

### **Key Analyses & Findings**

* **Top Math Schools**: Identified elite schools by filtering for an average math score of **640 or higher** (≥80% of the maximum score).
* **Top 10 Overall Schools**: Calculated a combined `total_SAT` score (Math + Reading + Writing) to rank and determine the **top 10 performing high schools** city-wide.
* **Borough Performance Spread**: Grouped data by borough and calculated the standard deviation of SAT scores to measure performance disparity. **Manhattan** was found to have the **largest score variation**, indicating the biggest performance gap between its schools.

### **Tools Used**

* **Python**
* **Pandas**
***


## [Project 3: Analysis of Student Exam Performance](https://github.com/Rafli-Alfiansyah/Factors-that-Fuel-Student-Performance)

This project uses **SQL** to analyze a student dataset to identify the key factors that influence exam scores, focusing on the relationship between study habits and academic outcomes.

* **Objective**: To determine the most significant predictors of student success by analyzing study hours, extracurricular activities, and exam results.
* **Method**: The analysis was conducted using SQL queries with data aggregation (`GROUP BY`, `AVG`), window functions (`DENSE_RANK`), and conditional logic (`CASE`) to segment and compare student groups.
* **Key Insight**: The number of **hours studied** showed the strongest positive correlation with higher exam scores. Students studying **16+ hours** averaged a score of **67.92**, significantly higher than the **62.63** average for those studying **1-5 hours**.

**Tools & Skills**: **SQL** (Data Aggregation, Window Functions, Conditional Filtering, Data Segmentation).
***


## [Project 4: The Search for the Golden Age of Video Games](https://github.com/Rafli-Alfiansyah/When-Was-the-Golden-Era-of-Video-Games-)

#### **Analysis & Key Questions**

Using SQL queries, this analysis aimed to answer several key questions:

* **What are the all-time best-selling games?**
    * *(Note: This query resulted in a `SyntaxError` and could not be completed, reflecting a real-world analysis challenge.)*
* **Which years produced the most critically acclaimed games?**
    * Calculated the average `critic_score` for each release year.
* **Which years qualify as a "golden age"?**
    * Identified years where either the average `critic_score` OR the average `user_score` was greater than 9.0.

#### **Key Findings**

* **1998 was the top year for critics**, boasting an average score of **9.32**.
* The data suggests a peak period for critical acclaim occurred around the turn of the millennium (**late 1990s - early 2000s**).
* Six "golden years" were identified where average review scores surpassed 9.0: **1997, 1998, 2004, 2008, 2009, and 2010**.

#### **Tools Used**

* **SQL**
***


## [Project 5: Analysis of Electric Vehicle Charging Habits](https://github.com/Rafli-Alfiansyah/Analyzing-Electric-Vehicle-Charging-Habits)

### **EV Charging Behavior Analysis**

This project uses **SQL** to analyze a dataset of EV charging sessions from apartment garages. The goal is to identify usage patterns and provide building managers with actionable recommendations to optimize station availability.

* **Objective**: To understand tenant charging habits to improve shared resource management.
* **Method**: The analysis answers three key questions by querying the `charging_sessions` table:
    1.  **Busiest Garages**: Identified by counting unique users (`COUNT(DISTINCT user_id)`).
    2.  **Peak Times**: Found by counting sessions per hour and day (`COUNT(*)`).
    3.  **'Super-Users'**: Flagged by finding users with an average charge time over 10 hours (`AVG(duration_hours)`).
* **Recommendations**: The findings suggest installing more stations in high-demand garages, implementing reservation systems for peak hours, and creating fair-use policies like idle fees to improve availability.

**Tools**: **SQL (PostgreSQL)**
***


## [Project 6: Motorcycle Parts Sales Analysis](https://github.com/Rafli-Alfiansyah/Analyzing-Motorcycle-Part-Sales)

### **Wholesale Revenue Analysis for Motorcycle Parts**

This project uses **SQL** to analyze sales data, calculating monthly net revenue from wholesale clients grouped by product line and warehouse.

* **Objective**: To provide the board of directors with a detailed wholesale revenue report for strategic decision-making.
* **Method**: A single SQL query was run to filter for wholesale clients, calculate net revenue (`total - payment_fee`), and group the results by product, month, and warehouse.
* **Insight**: The analysis successfully identified top-performing segments, such as the **Engine** product line at the **Central** warehouse in August, which generated **$9,528.71**.

**Tools**: **SQL**
***


## [Project 7:Analysis of Product Carbon Footprints by Industry](https://github.com/Rafli-Alfiansyah/Analyzing-Industry-Carbon-Emissions)

This project uses **SQL** to analyze a product emissions database, identifying which industry groups have the largest carbon footprints based on the most recent year of data.  GHG emissions from consumer products are a major contributor to climate change, and this analysis pinpoints the most impactful sectors. 🏭

#### **Method & Key Insight**

* **Objective**: To rank industries by their total CO2 equivalent emissions to inform sustainability efforts.
* **Method**: A single SQL query was executed to filter for the most recent year's data, `GROUP BY` industry, and `SUM` the `carbon_footprint_pcf` for each group.
* **Key Insight**: Heavy industries are the largest contributors. The **Materials** (107k tCO₂e) and **Capital Goods** (95k tCO₂e) sectors have the highest total carbon footprints in the dataset, highlighting them as key areas for environmental regulation.

#### **Tools Used**

* **SQL (PostgreSQL)**
* **Jupyter Notebook**
***


## [Project 8:Netflix Movie Analysis: A 1990s Throwback](https://github.com/Rafli-Alfiansyah/Investigating-Netflix-Movies)

This project uses **Python** to perform an exploratory data analysis on Netflix's library of movies from the 1990s. The goal was to uncover trends, such as typical film durations and niche genres, to inform a production company specializing in nostalgic content. 🎞️

#### **Method & Key Findings**

* **Objective**: To analyze movies from the 1990s on Netflix to find actionable insights for future film production.
* **Method**: Used the **Pandas** library to filter the `netflix_data.csv` dataset for movies released between 1990-1999. The analysis focused on movie durations and identifying specific sub-genres.
* **Key Insight**: The most common movie duration for 1990s films was **94 minutes**. A more specific filter also identified a niche of **7 short action movies** (under 90 minutes), providing valuable creative inspiration.

#### **Tools Used**

* **Python**
* **Pandas**
* **Matplotlib**
* **Seaborn**
***

## [Project 9:Sleep Health Data Analysis](https://github.com/Rafli-Alfiansyah/Getting-a-Good-Night-s-Sleep)
### **Analysis of Sleep Health and Lifestyle Data**

This project uses **Python** and **Pandas** to analyze a sleep survey dataset, aiming to uncover key relationships between lifestyle factors (like occupation and BMI) and sleep quality. 😴

#### **Method & Key Findings**

* **Objective**: To identify patterns in sleep health data that can provide actionable insights for improving user well-being.
* **Method**: The analysis involved grouping and aggregating the `sleep_health_data.csv` dataset to compare sleep duration, quality, and disorders across different occupations and BMI categories.
* **Key Insights**:
    * **Occupation**: **Sales Representatives** were identified as the profession with the lowest average sleep duration and quality.
    * **BMI & Insomnia**: A strong link was found between higher BMI and insomnia. Only **4%** of individuals with a 'Normal' BMI reported insomnia, compared to **43%** of those in the 'Overweight' category.

#### **Tools Used**

* **Python**
* **Pandas**
***

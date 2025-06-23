🚗 Vehicle Sales Data Cleaning Project
This project focuses on cleaning and preparing a real-world vehicle sales dataset to ensure it is suitable for analysis, visualization, and machine learning tasks.

📁 Dataset Summary
Original Columns Included:

year, make, model, trim, body, transmission, vin, state, condition, odometer, color, interior, seller, mmr, sellingprice, saledate

Source: Sourced from Kaggle or other publicly available data platforms.

🧽 Data Cleaning Steps
The following operations were performed using Python (Pandas) to clean and structure the dataset:

🔹 1. Dealing with Missing Data
Records missing essential fields like vin, sellingprice, or saledate were dropped.

Categorical nulls (like color, interior) were replaced with generic placeholders (e.g., 'unknown' or 'standard').

For numerical columns such as odometer and mmr, missing values were filled using the median.

Missing condition values were filled using the most frequent category (mode).

🔹 2. Duplicate Removal
Used .drop_duplicates() to eliminate repeated entries.

🔹 3. Text Normalization
Cleaned all string fields by converting them to lowercase and removing extra whitespace.

Standardized inconsistent terms within columns like transmission and condition.

🔹 4. Date Handling
Parsed the saledate column into a unified datetime64[ns, UTC] format.

Optionally formatted the date as dd-mm-yyyy for readability in exports.

🔹 5. Column Header Formatting
Renamed all column names using lowercase letters and underscores (_) to maintain naming consistency.

🔹 6. Corrected Data Types
Ensured all numeric columns (year, odometer, sellingprice, etc.) are in the correct integer or float format.

Validated that saledate is stored as a datetime object.

📂 Final Output
vehicle_sales_cleaned.csv — Cleaned CSV file

vehicle_sales_cleaned.xlsx — (Optional) Cleaned Excel version for external tools

⚙️ Tools & Technologies
Python

Pandas

Jupyter Notebook / VS Code

OpenPyXL (used for Excel output)

✅ What’s Next?
This dataset is now optimized for:

🔍 Exploratory Data Analysis (EDA)

📉 Data Visualization (e.g., using Seaborn or Matplotlib)

🤖 Machine Learning Projects (e.g., price prediction)

📊 Interactive Dashboards (in Power BI, Tableau, etc.)

👨‍💻 Author
Pratham Kumar Prasad
Aspiring Data Analyst | B.Tech Student | Passionate about Practical Learning

📝 License
Distributed under the MIT License.
You're welcome to use and modify this project as needed.

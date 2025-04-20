**Airbnb Data Cleaning and Analysis**

**Project Overview**

This project focuses on cleaning and analyzing an Airbnb dataset using Python. The dataset, sourced from Airbnb_Open_Data.csv, contains information about Airbnb listings, 
including prices, room types, neighborhoods, and reviews. The project involves data cleaning steps to handle missing values, duplicates, and formatting issues, 
followed by exploratory data analysis (EDA) with visualizations to uncover insights about listing distributions, pricing, and trends over time.

**Repository Contents**

  > **Airbnb_Open_Data.csv**: The raw dataset containing Airbnb listing information.

  > **Air Bnb.ipynb**: Jupyter Notebook with the complete data cleaning and analysis workflow.

  > **cleaned_data.csv**: The cleaned dataset output after processing.

  > **README.md**: This file, providing an overview of the project.


**Prerequisites**

To run the Jupyter Notebook, ensure you have the following Python libraries installed:
bash
pip install pandas numpy matplotlib seaborn

**Project Workflow**

1-**Data Loading**:
    > The dataset is loaded using pandas from Airbnb_Open_Data.csv.
    > Initial exploration is performed using df.head() and df.info() to understand the structure and identify issues.
    
2-**Data Cleaning**:
    > **Handling Missing Values**: Missing values in reviews per month are filled with 0, and last review is set to the minimum date. Rows with missing NAME or host name are dropped.
    > **Dropping Column**s: Unnecessary columns (license, house_rules) are removed.
    > **Formatting**: price and service fee columns are cleaned by removing $ and , symbols and converted to float.
    >**Removing Duplicates**: Duplicate rows are dropped to ensure data integrity.
    
3-**Exploratory Data Analysis (EDA)**:
    > **Price Distribution**: A histogram visualizes the distribution of listing prices.
    > **Room Type Distribution**: A count plot shows the frequency of different room types (e.g., Entire home/apt, Private room).
    > **Neighborhood Analysis**: A count plot displays the number of listings by neighborhood group.
    > **Price vs. Room Type**: A boxplot explores the relationship between room types and prices.
    > **Reviews Over Time**: A line plot tracks the number of reviews over time, aggregated by month.
    
4-**Output**:
    > The cleaned dataset is saved as cleaned_data.csv.

**How to Run**

1. Clone this repository:
   bash
   git clone https://github.com/your-username/airbnb-data-cleaning.git

2. **Navigate to the project directory**:
  bash
  cd airbnb-data-cleaning

3. **Install dependencies**:
  bash
  pip install -r requirements.txt
  (Optional: Create a requirements.txt with pandas, numpy, matplotlib, seaborn if desired.)

4. **Open the Jupyter Notebook**:
   bash
   jupyter notebook Air\ Bnb.ipynb
   
6. Run the notebook cells to execute the data cleaning and analysis.

**Visualizations**

The notebook includes the following visualizations:
    > **Price Distribution**: Histogram of listing prices with a kernel density estimate (KDE).
    > **Room Type Distribution**: Count plot showing the prevalence of room types.
    > **Listings by Neighborhood**: Count plot of listings across neighborhood groups.
    > **Price vs. Room Typ**e: Boxplot comparing price distributions across room types.
    > **Reviews Over Time**: Line plot of review counts by month.
    
**Key Insights**
    > The dataset contains 101,410 unique listings after cleaning.
    > Most listings are Entire homes/apts (53,132) or Private rooms (45,967).
    > Prices range from $50 to $1,200, with a mean of approximately $625.
    > Neighborhood groups like Manhattan and Brooklyn dominate the listings.
    > Review activity varies over time, as shown in the temporal analysis.
    
**Future Improvements**
    > Handle remaining missing values in columns like host_identity or country.
    > Add more advanced visualizations, such as geographic maps using lat and long.
    > Perform statistical analysis to identify factors influencing pricing.
    > Incorporate machine learning models to predict listing prices or review rates.

  
**Dataset Source**
    > The dataset is assumed to be sourced from a public repository or Kaggle (e.g., Airbnb Open Data). Ensure proper attribution if required.

**License**
    > This project is licensed under the MIT License. See the  file for details.

**Contact**
    > For questions or suggestions, feel free to open an issue or contact your-naushadsaifi12345@gmail.com.

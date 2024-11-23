# Vehicle Sales and Market Trends Analysis
![Vehicle Sales Analysis](images/cars.jpg)
## Introduction
In the rapidly evolving automotive industry, understanding market trends and vehicle sales dynamics is crucial for manufacturers, dealers, and consumers. The "Vehicle Sales and Market Trends Dataset" provides a comprehensive collection of information pertaining to the sales transactions of various vehicles. This dataset encompasses details such as the year, make, model, trim, body type, transmission type, VIN (Vehicle Identification Number), state of registration, condition rating, odometer reading, exterior and interior colors, seller information, Manheim Market Report (MMR) values, selling prices, and sale dates.

This study aims to explore and analyze this dataset to uncover valuable insights into vehicle sales patterns and market trends. By performing exploratory data analysis (EDA), data cleaning, preprocessing, and visualization, it is aimed to identify key factors influencing vehicle prices, detect outliers, and understand the distribution of various attributes. Additionally, feature engineering and selection techniques will be applied to enhance the dataset's utility for machine learning models, ultimately aiding in predictive analytics and decision-making processes.

Vehicle Sales Dataset: [Vehicle Sales Data](https://www.kaggle.com/datasets/syedanwarafridi/vehicle-sales-data)

Check The Notebook on Kaggle: [Comprehensive Vehicle Sales Data Analysis](https://www.kaggle.com/code/yigitcanakcay/comprehensive-vehicle-sales-data-analysis)

## Dataset Information
The dataset contains the following columns:
-  **year**: Manufacturing year of the vehicle (int64)

-  **make**: Vehicle manufacturer (object)

-  **model**: Vehicle model name (object)

-  **trim**: Trim level (object)

-  **body**: Body style (object)

-  **transmission**: Transmission type (object)

-  **vin**: Vehicle Identification Number (object)

-  **state**: Location state (object)

-  **condition**: Numeric rating of the vehicle's condition (float64)

-  **odometer**: Mileage reading (float64)

-  **color**: Exterior color (object)

-  **interior**: Interior color/material (object)

-  **seller**: Seller information (object)

-  **mmr**: Manheim Market Report value (float64)

-  **sellingprice**: Final sale price (float64)

-  **saledate**: Date of sale (object)

  

## Exploratory Data Analysis (EDA)

  

### Initial Data Inspection

  

- Loaded the dataset and displayed the first few rows.

- Checked the general information and data types of the columns.

- Identified numerical and categorical columns.

  

### Descriptive Statistics

  

- Generated descriptive statistics for numerical columns.

- Created a function to print detailed statistical information for numerical columns.

  

### Data Cleaning and Preprocessing

  

- Checked for missing values and calculated the percentage of missing values for each column.

- Added missing values on purpose to simulate real-world scenarios.

- Visualized missing data using `missingno` package (bar chart, matrix, heatmap, dendrogram).

  

### Handling Missing Values

  

- Filled missing values for numerical columns with the mean value grouped by the 'make' column.

- Filled missing values for categorical columns with the mode value.

- Dropped rows with remaining missing values.

  

### Outlier Analysis

  

- Identified outliers using the interquartile range (IQR) method.

- Removed outliers and verified the impact on the dataset.

  

### Data Visualization

  

- Plotted bar plots for categorical columns showing the top categories.

- Created pie charts for categorical columns to show the distribution of top categories.

- Generated scatter plots to visualize the relationship between categorical features and selling prices.

- Plotted histograms for numerical columns to understand their distribution.

- Created boxplots to identify outliers in numerical columns.

- Visualized the correlation between mmr and selling prices using scatter plots.

  

## Feature Engineering and Selection

  

- Removed unnecessary columns ('vin' and 'saledate') from the dataset.

- Generated a new feature 'mmr_sellingprice' by dividing the 'mmr' column by the 'sellingprice' column.

- Applied one-hot encoding to the 'transmission' column.

- Applied frequency encoding to the remaining categorical columns.

- Normalized numerical columns using MinMaxScaler.

  

## Conclusion

  

This study provided a comprehensive analysis of the Vehicle Sales and Market Trends Dataset. By performing EDA, data cleaning, preprocessing, and visualization, we gained valuable insights into vehicle sales patterns and market trends. Feature engineering and selection techniques were applied to enhance the dataset's utility for machine learning models. The resulting dataset is now ready for predictive analytics and decision-making processes.

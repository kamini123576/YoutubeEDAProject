# YoutubeEDAProject

**Overview** <br>

This project performs Exploratory Data Analysis (EDA) on a dataset containing information about YouTube channels. The dataset includes columns such as Rank, Grade, Channel Name, Video Uploads, Subscribers, Video Views, and more. The goal is to clean the data, analyze key metrics, and derive meaningful insights regarding channel performance and grading.

**Steps**<br>
**Import Libraries and Load the Dataset:** <br>
. Libraries like pandas, seaborn, and matplotlib are used for data manipulation and visualization.<br>
. The dataset is loaded from Google Drive into a Pandas DataFrame.<br>

**Initial Exploration:** <br>
. Display the first and last few rows of the dataset.<br>
. Retrieve basic information such as shape, column data types, and memory usage.<br>

**Data Cleaning:** <br>
. Handle missing values:<br>
  .  Replace invalid values (like --) with NaN.<br>
  . Visualize missing data using a heatmap.<br>
  . Drop rows with missing values.<br>
. Clean specific columns:<br>
  . Remove non-numeric characters (e.g., st, nd, th) and commas from the Rank column and convert it to an integer.<br>
  . Convert Subscribers and Video Uploads to integers.<br>
. Map categorical values in the Grade column to numeric values for easier analysis.<br>

**Feature Engineering:** <br>
. Calculate a new column Average_views, defined as Video views / Video Uploads.<br>

**Data Analysis:** <br>

. Identify the top channels based on Video Uploads.<br>
. Compute the correlation matrix to find relationships between numeric variables.<br>
. Visualize key insights using bar plots:<br>
  . Grade vs. Video Uploads<br>
  . Grade vs. Average Views<br>
  . Grade vs. Subscribers<br>
  . Grade vs. Video Views<br>

**Summary and Conclusion <br>
.  Key Findings:** <br>

1. Channels with a higher grade (e.g., A++) perform better in terms of subscribers, video views, and average views.<br>
2. A strong positive correlation exists between Subscribers and Video Views.<br>
3. The Rank column was successfully cleaned to facilitate analysis.<br>

. **Dataset Cleaning and Transformation:** <br>

. Non-numeric characters and invalid values were handled effectively.<br>
. Numeric conversions ensured the dataset was suitable for statistical analysis.<br>

. **Visual Insights:** <br>

. Bar plots revealed how grading directly impacts the performance metrics of YouTube channels.<br>

**Next Steps:** <br>
. Conduct more in-depth analysis to predict channel success based on other factors.<br>
. Investigate the influence of content type on grading and performance metrics.<br>

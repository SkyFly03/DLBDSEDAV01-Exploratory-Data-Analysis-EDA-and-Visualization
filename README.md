# DLBDSEDAV01 – Exploratory Data Analysis (EDA) and Visualization  
## Task 1: Visually Exploring a Dataset  

## Qatar Airways Reviews – EDA Project Overview

This project uses Exploratory Data Analysis (EDA) to examine reviews of Qatar Airways from Kaggle.  
The goal is to show trends and patterns in customer feedback using visualizations and statistical techniques.

---

## 1. Dataset Overview

**Source**: [Kaggle – Qatar Airways Reviews](https://www.kaggle.com/datasets/pranaybshah/qatar-airways-reviews)  
    
**Main Columns**:
- `rating`: Customer rating from 1 to 10  
- `review`: Written feedback from passengers  
- `aircraft`: Aircraft model  
- `seat_type`: Economy, Business, or First Class  
- `date_published`: When the review was posted  
- `route`: Flight path (origin to destination)  
- `recommended`: Whether a passenger recommends Qatar Airways

---

## 2. Project Objectives

- Show how customer satisfaction is distributed  
- Compare service quality across cabin classes  
- Track rating trends over time  
- Analyze common themes in customer feedback  
- Study how delays and flight details affect ratings  
- Visualize satisfaction by aircraft, nationality, and traveler type

---

## 3. Setup: Installation and Library Imports

Standard Python libraries used:
- `pandas`, `numpy`, `plotly`, `matplotlib`, `seaborn`  
- `nltk` for basic text analysis  
- All code was run in a local Jupyter Notebook via Anaconda

---

## 4. Data Processing and Transformation

### 4.1 Data Cleaning
- Removed duplicate rows  
- Standardized column names  
- Dropped rows with missing key values (rating, seat_type, or review)

### 4.2 Transformation
- Converted `date_published` to datetime  
- Grouped similar aircraft types and standardized categorical data

### 4.3 Focus Variables
- **Numerical**: `rating`  
- **Categorical**: `seat_type`, `type_of_traveller`, `aircraft`  
- **Datetime**: `date_published`

---

## 5. Exploratory Data Analysis & Visualization

### 5.1 Overall Satisfaction
- Histogram and box plot showed that most passengers rated their experience between 8 and 10.
- Key statistics:  
  Mean: 7.31 | Median: 8.0 | Mode: 10 | Std Dev: 2.86 | IQR: 5
  ![image](https://github.com/user-attachments/assets/74614b5c-0b56-4562-8027-d77f968f1be9)

### 5.2 Ratings by Cabin Class
- Violin plots revealed that Economy ratings are more spread out and often lower.
- Business and First Class showed consistent high satisfaction.
- ANOVA test confirmed statistically significant differences.
![image](https://github.com/user-attachments/assets/9fa8d244-4857-4e12-bf7d-0b1a867312fd)

### 5.3 Trends Over Time
- Scatter plot with regression line showed a slight decrease in satisfaction over time.
- Density heatmaps were tested but not used due to low readability.
![image](https://github.com/user-attachments/assets/5a783167-2d99-462d-8db6-d4c705b2b026)

### 5.4 Common Themes in Comments
- Bar chart showing top 20 frequent words like “crew”, “delay”, and “food”.
- Word clouds were tested but replaced for better clarity.
![image](https://github.com/user-attachments/assets/05d06102-5169-471b-94fb-520ca59896c5)

### 5.5 Impact of Delays
- Grouped histogram compared ratings with and without delay mentions.
- T-test confirmed that delay-related reviews have lower ratings on average.
![image](https://github.com/user-attachments/assets/e32a42b1-f518-444c-897e-0a9f0b71add6)

### 5.6 Satisfaction by Aircraft, Traveler, Country, and Seat
- Bubble chart subplots visualized average ratings and review count across groups.
- Newer aircraft scored higher, Business travelers rated lower, and German passengers rated lowest.
![image](https://github.com/user-attachments/assets/407e829e-4aee-4f5a-aa2d-4e1c5a3f0f13)

---

## 6. Conclusion

### Summary of Key Insights:
- Business and First Class receive the highest satisfaction scores.
- Newer aircraft models (A350, A380) are associated with better ratings.
- Business travelers and German passengers are less satisfied than others.
- Ratings are generally high, but improving Economy Class could boost satisfaction further.

### Strategic Recommendations:
- Improve Economy Class service  
- Modernize older aircraft  
- Investigate causes of lower satisfaction among German passengers  

---

## 7. View Notebook with Visual Output

GitHub may not render large notebooks. Use [NBViewer](https://nbviewer.org) to open the notebook directly:

**https://nbviewer.org/github/SkyFly03/DLBDSEDAV01-Exploratory-Data-Analysis-EDA-and-Visualization/blob/main/Qatar%20EDAV.ipynb**  

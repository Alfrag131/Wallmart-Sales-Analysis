# Wallmart Sales Analysis

1. Importing Necessary Libraries and Data
   
2. First Look to Data and Merging Dataframes

         #weekly ave sales 
         storemean=df.groupby(by='Store').mean(numeric_only=True)
         storemean.head(3)

4. Exploratory Data Analysis (EDA)
   
   1. Sales By Store Type

  ![image](https://github.com/user-attachments/assets/bae1b918-515f-4215-9d35-42cc93d39dfd)

      Findings:
      - Clear seasonality around holidays (notably Thanksgiving and Christmas)
      - Store Type A consistently outperformed B and C in sales
      - Store size correlates with type, affecting capacity and reach

  2. Mean Sales by Department

 ![image](https://github.com/user-attachments/assets/e3d01aa8-086b-4e01-9756-85deedb673bf)

      Findings:
      - Certain departments (e.g., electronics, groceries) generate higher sales
      - Opportunities to optimize underperforming departments

   3. MarkDown Trends Over Time

  ![image](https://github.com/user-attachments/assets/0e28bbe3-f332-4153-b904-e8e4692bdae8)

      Findings:
      - Spikes in markdowns are often followed by increases in sales
      - Suggests markdowns are used strategically around sales events and holidays

   4. Sales By Temperature

  ![image](https://github.com/user-attachments/assets/fa77e74c-cd70-468c-83fe-5bc77adb3804)

      Findings:
      - Mild temperatures (around 40–50°F and 70–80°F) are associated with higher weekly sales, suggesting that moderate weather encourages more in-store shopping and holidays
      - Extremely cold or hot temperatures (below 30°F or above 85°F) often coincide with reduced sales, possibly due to customers avoiding travel or adverse weather conditions

   5. Smoothed CPI with Trend by Store Type

  ![image](https://github.com/user-attachments/assets/8db2773a-b4d5-4176-be5b-01a49e26be75)

      Findings:
      - The overall CPI trend is similar across store types, indicating that inflation and economic factors impact all store categories in comparable ways
      - For Store Types A and B, there is a clear positive trend — the Consumer Price Index gradually increases over time, suggesting these store types are more sensitive to economic changes
      - In contrast, Store Type C shows a less pronounced or nearly flat trend, possibly reflecting more stable conditions, differences in store size, or departmental composition within this type

   6. Smoothed Unemployment with Trend by Store Type

  ![image](https://github.com/user-attachments/assets/7a498ead-1fa8-4569-9a4e-25e6a3548a67)

      Findings:
      - Overall, the unemployment rate fluctuates but exhibits clear differences in trends across store types, generally showing a downward trend
      - Store Types A and B display a nearly flat yet slightly downward trend, indicating relatively stable and improving unemployment conditions for these segments
      - In contrast, Store Type C shows a pronounced downward trend, possibly reflecting stronger improvements in local employment conditions for this category

   7. Sales Forecast for the Year

  ![image](https://github.com/user-attachments/assets/0564795b-00dc-4082-9b0c-c51c556f0d2c)

      Findings:
      - The Prophet model effectively forecasts total weekly sales for the upcoming year (365 days), capturing seasonal patterns and trends from historical data
      - The forecast shows distinct seasonal peaks likely corresponding to holiday periods and sales events (e.g., Christmas, Black Friday)








  

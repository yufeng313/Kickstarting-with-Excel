# Kickstarting-with-Excel
## Overview of Project
   This project is mainly helping our client,Louise,to visualize campaign outcomes based on several parameters,and will finally give Louise a reference to  her crowdfunding campaign with her play,Fever.
### Purpose
   In this challenge, I'll create two charts to describe the relationship between outcomes and launch datas,and the relationship between outcomes and funding goals, and then analyze the dataset to see how launch dates and funding goals affect the outcomes of the compaign. 
## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
    1.I created a new column labeled "Years" in the Kickstarter worksheet,and extract the year from the “Date Created Conversion” column. Then Create a pivot table to a new sheet.
    2.In order to see the outcomes based on launch data, I drag "outcomes" to the column, and "Data Created Conversion" to the row,and then drag "outcomes" to the Values.Filter the pivot table based on "Parent Category" and "Years."
    3.Then create a line chart from the pivot table to visualize the relationship between outcomes and launch month.
    Here are the pivot table and pivot chart:
    ![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/107179765/173181288-0d186b25-9a7c-4a31-bb88-6d91eb5ef12c.png)

### Analysis of Outcomes Based on Goals
    1.I created a new sheet with several columns to calculate the total projects amount,and the percentage of successful,failed,canceled projects based on each goal-amount ranges. 
    2.Use those data to create a line chart ,to visualize the relationship between the goal-amount ranges and the percentage of successful, failed, or canceled projects.
    Here is the line chart:
    ![Outcomes_vs_Goals](https://user-images.githubusercontent.com/107179765/173203184-98216aac-6613-45a8-8dfe-0d87a2a4cb98.png)

### Challenges and Difficulties Encountered
    1.In the "Analysis of Outcomes based on Launch Date", when I drag "Data Created Conversion" to the row, it shows 3 things: "Data Created Conversion", "Quarters", "Years2" at the same time. I noticed there's a "Years2" in the pivot field.And I'm not sure the difference between "Years" and "Years2", so I drag "Years2" and "Quarters" out of the column.
    2.In the "Analysis of Outcomes based on Goals", when I calcuted the percentage of the successful, I applied the formula:=B2/E2,and change the data format from Genaral to Percentage. There are still two numbers after the decimal. And then I tried to use the ROUND funtion we've learned in the Module 1 before, but got the wrong data, so I went back to the format cell and specifies how many numbers after the decimal will be viewed. Also I changed the color of the line chart to make it looks more directly.
    
## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
  1.From the line chart,we can see three different lines,the line trends of successful and failed are almost display in the same way,while the rate of the successful campaign increased,the rate of the failed campaign also increased; while the rate of the successful campaign decreased,the rate of the failed campaign also decreased. So we can conclude that the rate of successful and failed campaigns are proportional.
  2.Another conclusion ,you can find there's a spike at May,and the months of May and June both have a greater success rate, while the failed rate had roughly the same number,so we can conclude that the month of May would be a good recommendation for launching a theater production. Besides,winter season is not a good quarter to launch the campaign,for the low successful rate and high failed rate, especially in Dec.
  
- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?

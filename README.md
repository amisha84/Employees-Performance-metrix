# Employees-Performance-metrix
For making dashboard first be insure that is your data should be clean properly.
The base on data i have create the dashboard regarding employees performance there age and bases on gender.
I have use multiple chats and KPIs for showing the total employees,there age,average salary and other details.
For calculating age group i used mention DAX formula,
Age Group = 
SWITCH(
   TRUE(),
   [Age] >= 0 && [Age] <= 18, "0-18",
   [Age] >= 19 && [Age] <= 30, "19-30",
   [Age] >= 31 && [Age] <= 40, "31-40",
   [Age] >= 41 && [Age] <= 50, "41-50",
   [Age] >= 51 && [Age] <= 60, "51-60",
   [Age] > 60, "60+",
   "Unknown"
)

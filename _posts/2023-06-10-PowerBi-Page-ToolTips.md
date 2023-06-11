## Maximizing Customer Insights with Power BI's Page Tooltips

### Introduction
In the world of data analysis and visualization, tools that offer interactive and immersive experiences are highly valued. Power Bi is one such data visualization tool where reports created through the software offer a multitude of interactive abilities for the report user. 

One of my favorite interactive capabilities is [Power Bi’s Page Tooltips](https://learn.microsoft.com/en-us/power-bi/create-reports/desktop-tooltips?tabs=powerbi-desktop).
These are tooltips that show an additional, smaller page when a value is hovered over. By incorporating page tooltips into your Power BI reports, you can bring additional layers of information to your visualizations, enabling users to delve deeper into the data and extract valuable insights.
<br>

---

### Example: Using Page Tooltips to show Volunteer Insights
All Data used to create this Volunteering report is fake and generated using the random functions on google sheets. Feel free to download the spreadsheet [here](https://github.com/KarissaLowe/KarissaLowe.github.io/blob/main/ExampleData/EventData_PowerBiTooltips.csv) to practice with!

In this example, I used a Page Tooltip to display the donation amount category volunteers are part of broken down by which volunteer activity they are involved with. 
Are there certain volunteer activities that create a stronger connection with the organization’s mission? Why might certain activities attract individuals who already donate?

Here is how the report looks initially:

![ToolTip Report Page Example](https://github.com/KarissaLowe/KarissaLowe.github.io/blob/main/Images/Tooltip_Image1.PNG?raw=true)


Using Page Tooltips, the user can hover over the table to see the donation category of volunteers involved in each activity:

![ToolTip Report Page Example User is hovering over a value to see tooltip 1](https://github.com/KarissaLowe/KarissaLowe.github.io/blob/main/Images/Tooltip_Image2.PNG?raw=true)
![ToolTip Report Page Example User is hovering over a value to see tooltip 2](https://github.com/KarissaLowe/KarissaLowe.github.io/blob/main/Images/Tooltip_Image3.PNG?raw=true)
<br>

---

### Other Tooltip Ideas
Here are a few other ideas on how to use Page Tooltips to drive more customer insight:

1. Customer Profiling:
   - By hovering over a customer data point, you can display a tooltip that includes details such as demographics, purchase history, customer preferences, and other relevant attributes.
2. Donation Patterns:
   - By incorporating tooltips into your donation visualizations, you can display details about each donation, including the amount, date, campaign, and any associated notes. This allows you to identify patterns and trends in donation behavior, such as peak donation periods or preferred campaigns. Or look more closely into outliers.
3. Geographic Insights:
   - If your data includes geographic information, page tooltips can be utilized to provide localized insights. For example, you can display tooltips that show regional sales performance when the user hovers over a specific area.

By implementing effective page tooltips, you can empower your audience to interact with your data in a more meaningful way, giving the user more ownership in uncovering insights and using the data.

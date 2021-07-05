# An Anlysis of Kickstarter Campaigns - Module 1

# **Overview**  

  This is a look at a dataset from past kickstarter campaigns to determine if there are any insights to be gleamed and hopefully predict some things that could be done on a future kickstarter campaign to make it successful.  This dataset was sent to us by a client looking to do their own kickstarter campaign for a play.  We were given a raw dataset that needed some cleaning up and breaking down before proper analysis could be done to really focus on the specific type/category of kickstarter campaign that the client needed.  Upon filtering and visualizing the data, some insights were gained, either with a graph or statistical calculations, that we could then forward to the client.  
  
# **Analysis and Challenges** 

  **Category Breakdown**

   After getting the dataset cleaned up and ensuring all data was readable, certain analysis was done on the data.  First and foremost, we focused data that was in the US since the client said that is where the play would be.  Next we moved to create some visuals to better understand that data.  First one being was the "Theater" category even successul at all.
   
https://github.com/wprich/KickStarter-AnalysisM1/blob/main/Resources/ParentCategoryOutcomesCBC.png
![ParentCategoryOutcomesCBC](https://user-images.githubusercontent.com/85487722/124496927-f581d600-dd6e-11eb-941f-f26604446707.png)

  According to the graph, the theater category is the most successful out of all the others.  In fact, out of all the total theater kickstarter campaigns, 912, there were 525 successful.  
  
  **Subcategory Breakdown**
  
  We can break this down even further since our client more specifically wants to fund a play, which is a subcategory of theater.  
https://github.com/wprich/KickStarter-AnalysisM1/blob/main/Resources/SubCategoryOutcomesCBC.png
![SubCategoryOutcomesCBC](https://user-images.githubusercontent.com/85487722/124497628-fa935500-dd6f-11eb-8b2d-4e17cee73697.png)

  This shows us that number of successful play kickstarters is definitely more than half.  This tells us that there is a good chance this clients kickstarter campaign for her play can be influenced to succeed as long as proper steps are taken.  But in order to find out what those steps need to be, we must do more analysis.  
  
  **Launch Dates effect on Outcome**
  
  One key factor in any launch of a product/idea is timing.  When would be the best time to launch a kickstarter campaign and when would be the worst?  After filtering the data to show us the "Theater" category, we could then break it down into the months to see which months had the most success and which had the most failed.
https://github.com/wprich/KickStarter-AnalysisM1/blob/main/Resources/Theater_Outcomes_vs_Launch.png

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/85487722/124498580-6f1ac380-dd71-11eb-9816-0c7fa4fdf94d.png)

  This graph shows us that the months with the most successful theater campaigns are May, June, and July in that order.  The months with the least are January, March, September, November, and December.  Also, the month with the most failed campaigns is October.  This seems to follow a trend of people not spending much money during the winter holidays and spending more money during the middle of spring and/or start of summer.  
  
**Goal Amounts effect on Outcome**

  One of the last graphs made was to look at the relationship between the stated goal amount, or the amount the kickstarter campaign asked for, to how well they were funded.  Were the campaigns who asked for the most successful or unsuccessful?  What abou the least?  After filtering the data to only look at the "plays" subcategory of "theater",  the data was then broken up into Goal amounts seperated in 5,000 dollar increments.  
https://github.com/wprich/KickStarter-AnalysisM1/blob/main/Resources/Outcomes_vs_Goals.png
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/85487722/124499546-0df3ef80-dd73-11eb-9a87-a00e6502087f.png)

  This last graph tells the client that as long as she asks below a certain amount of capital, around 4,000 dollars, she has roughly a 70% chance to be fully funded.  
  
**Challenges**

   There weren't any particular challenges that stand out from the typical in this project.  One challenge that most could encounter would be not understanding what the statistical methods are telling them.  
https://github.com/wprich/KickStarter-AnalysisM1/blob/main/Resources/Descriptive%20Statistics.png
![Descriptive Statistics](https://user-images.githubusercontent.com/85487722/124501158-e94d4700-dd75-11eb-9b2d-4539c4f202c0.png)

  These calculations show us the statistics based on US Kickstarters only.  It tells us that mean for the goal and the mean for the pledged seem to be close together.  Same for the median of the goal and median of the pledged.  While the standard deviation seems to be high for either category, pledged and goal, this may be an indication of skewedness in our data or some big outliers are affecting the data set.  It seems that if our client can keep the goal at or below 3,000 dollars, they stand a good chance at being funded.  If the cost or goal goes to 5,000 dollars or higher, the chances of being funded decreases significantly.

# **Results and Limitations**

**Conclusions**
  
  One conclusion that can clearly be drawn from the "Theater Outcomes by Launch Date" chart, is that the most successful month for a kickstarter campaign of the category is May.  So our client should plan to launch their kickstarter around that time.  Another conclusion is that the client should also avoid pushing the kickstarter until October as that is the worst month and has the greatest number of failed kickstarters.  Again, this falls in line with people tend to spend their money and go out more during the mid spring to summertime and save money closer to holidays since they will be shopping for gifts.   
  Another conclusion that can be drawn from the "Outcomes based on Goals" chart is the client should keep their cost/goal amount down to probably as low as possible.  3,000 dollars or less would be ideal but should stay away from approaching or going over 5,000.  Reason being is the percentage of failures start to increase the higher the goal amount is.  
  
**Limitations**

   As with any data set, this one had some limitations.  For instance, the data set gave us all kickstarter campaign data seperated by country.  Countries are big places,  does the client plan to hold the play in Central Park in New York City?  Or at a community college in Charlotte, North Carolina?  These regional distinctions can have some impact on cost of production as well as availability of capital.  We could break down the regions from the countries into pivot tables that allow us to sort by the state and/or region in the US and different regions in other countries.  Another limitation is there seem to be some outliers in the data that have shown to skew the data.  One of which being project ID 122, The Time Jumper (Canceled), which had a goal amount of 100,000,000 dollars and a pledge amount of zero.  My recommendation is that this data point be dropped from the set.  This will give us a better grasp of what the data is telling us as well as a better picture over what makes a kickstarter a success or failure.  We could also use more graphs to show us the skew of the data visually, to see if the skew is more left or right leaning.    

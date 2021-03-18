# kickstarter-analysis

#Kickstarter Analysis


I reviewed the data to assist the Kickstarter Campaign with finding trends on fundraising for Theater projects. 

##Analysis
I started with familiarizing myself with the raw data and making the necessary format changes. I applied some conditional formatting changes and time conversion. 

I created a Pivot table with outcomes and filtered to just show Theater Outcomes. 

=GETPIVOTDATA("outcomes",'Theater Outcomes by Launch Date'!$A$4,"outcomes","successful","Date Ended Conversion",1)

 ![Theater Outcomes by Launch Date]


I used the CountIfs formula to capture the data needed for the Outcomes Based on Goal chart. 

=COUNTIFS(Kickstarter!$F:$F,"successful",Kickstarter!$D:$D,"<=1000",Kickstarter!$R:$R, "plays")
=COUNTIFS(Kickstarter!D:D,">=1000",Kickstarter!D:D, "<=4999", Kickstarter!F:F,"successful",Kickstarter!R:R, "plays")

![Outcomes Based on Goal]
 

##Results

###Based off the analysis of the Theater Outcomes by Launch Date:
	*There were more Successful Theater Outcomes than Failed Outcomes.
 *Campaigns during the summer months had a higher success rate.

###Based off the analysis of the Outcomes based on Goals:
*Theater performances had a higher rate of success if the fundraising Goal was less than $1999.00. 

###The Data that was provided had some limitations. 
*If the times of the Theater performance had been provided, I could have reviewed which show times had the highest rate of attendance for use in future campaigns. 

*Other graphs that could be useful for the Kickstarter Campaign would be the analysis of the % Funded column to determine which Category / Subcategory had the highest % Funded amount.  The results could be shown in a pie chart to provide another type of visual for the presentation. 

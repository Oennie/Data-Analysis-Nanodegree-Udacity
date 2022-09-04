# FBI Gun Data Exploration

## Dataset
**Analysing data from the FBI's National Instant Criminal Background Check System (NICS) and US Census Data**

The NICS [data](https://www.fbi.gov/file-repository/nics_firearm_checks_-_month_year_by_state_type.pdf/view) provides information on transaction submitted to NICS in order determine whether a prospective buyer is eligible to buy firearms or explosives. This is important to ensure that each customer does not have a criminal record or is eligible to make a purchase. 

The US Census [data](census.gov) contains several variables at the state level like population.

## Summary of Findings
We looked at the datasets from the *FBI's National Instant Criminal Background Check System (NICS)* and *US Census Data* then explored the following questions:

 + Which states have the highest transactions submitted for background checks?
 + Is there a growth in attempt to purchase firearms from 1998 till 2017?
 + Which gun type is preferred?
 + Are more/less populated areas likely to purchase more firearms?
---
Here are the findings from the exploration carried out:

1. **Which states have the highest transactions submitted for background checks?**

+ When the total number of checks submitted is looked at we see the following 10 states have the highest submission:
        Kentucky, Texas, California, Illinois, Pennsylvania, Florida, Ohio, North Carolina, Indiana and Tennessee
+ When we look at the total number of transactions submitted per population, we have the following top 10 states:  
        Kentucky, Montana, West Virginia, Alaska, Wyoming, Utah, South Dakota, Alabama, Arkansas and North Dakota

2. **Is there a growth in attempt to purchase firearms from 1998 till 2017?**
+ We can see a rising trend in the number of backgorund checks submitted from 1998-2016 which may indicate a growth in attempt to purchase a firearm but a sharp decline in 2017. The decine may not necessarily mean the number is dropping but can be because of incomplete period as we only have 9 months of data for 2017

3. **Which gun type is preferred?**
+ There seem to be a higher background check submission for long guns which may suggest individuals attempt to purchase that type more over hand guns
+ Looking at pre-pawned and redemption hand and long guns we also see higher checks submission for both pre-pawned and redemption long guns which could suggest the preference for long guns over hand guns

4. **Are more/less populated areas likely to purchase more firearms?**
+  It looks like there is a strong relationship between the number of population and total background checks submission so the higher the poulation the more transactions submitted
***
**Limitations**
> - The analysis carried out uses descriptive statistics not inferetial, no hypotheses or controlled experiments was created with the data.
>
> - All columns with over 2000 missing values were dropped in the FBI's NCIS dataset, this could have been filled with various some values e.g mean. This did not allow us to carry out exploration on these columns and understand the relationships.
>
> - The FBI's NCIS dataset has incomplete period (only 9 months data) for the year 2017 which does not allow us to properly understand the trend of gun submission checks over the years.
>
> - Only the population for 2016 was taken from the US Census dataset, other variables could have helped explore more relationships like checks submitted by different age groups



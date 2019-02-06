# National Longitudinal Survey of Youth 1997

The data we are using comes from the [National Longitudinal Survey of Youth 1997](https://www.nlsinfo.org/content/cohorts/nlsy97) (NLSY97), conducted by the US Bureau of Labor Statistics. The first wave of the NLSY97 surveyed respondents who were aged 12-17 in 1997. These same individuals are re-interviewed each year, making this a *longitudinal* study.

I created an extract of the full NLSY97 data using the [NLS Investigator](https://www.nlsinfo.org/investigator/pages/login.jsp). We will look at educational attainment among individuals still present in the most recent wave of 2015-2016. I have removed any individuals from the sample who had not completed high school by 2008. So we are basically looking at the probability of attending and completing college by 2015-16 among respondents who had completed high school by 2008. Here is a full description of all variables in the dataset that we will use.

- **gender**: gender of the respondent recorded only as male or female. 
- **race**: race of the respondent: white, black, Latino, Asian/Pacific Islander, American Indian, other. Information here is based off of responses during the screening interview with a household informant and is not self-reported. 
- **family_type**: What type of family does the respondent currently reside in? I have combined two biological and two adoptive parents into a single family type. The other types are a two parent household with one step-parent (bio + step), a single biological parent, and all other cases.
- **hh_income**: The household income for the respondent's household, measured in 1000's of US dollars.
- **hh_networth**: The net worth of the respondent's household, measured in 1000's of US dollars. Note that this value can be negative.
- **high_parent_ed**: the highest years of schooling reported by the respondent's resident parents and/or biological parents.
- **attend_college**: If the respondent reported at least one year of college attendance this variable is recorded as a 1, and a 0 otherwise.
- **complete_college**: If the respondent reported completion of a four-year bachelor's degree, this variable is a recorded as a 1, and a 0 otherwise. 

In the original data, there are missing values for some observations on some of these variables. To simplify our analysis, I have used some advanced techniques that are beyond the scope of our class to impute these missing values.

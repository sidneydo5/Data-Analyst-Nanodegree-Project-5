# Airport Data Exploration
## by Sidney D. Osborn


## Dataset (Link: https://video.udacity-data.com/topher/2023/July/64ac0f4a_ot_delaycause1_dl-2/ot_delaycause1_dl-2.zip)

> This dataset was taken from the U.S. DOT wesite and provides information on airline flight delays, cancellations and other similar information. It covers years 2013-2023.
> There are 21 features in the Airport dataset. with just over 338,000 rows containing information for individual flights.
> Here's a breakdown of what the columns are (in alphabetical order) given by the dataset orignator:
- 'airport': 'Airport Code for Arrival Airport',
- 'airport_name': 'Airport Name',
- 'arr_cancelled': 'Number of cancelled flights',
- 'arr_del15': 'Total number of delayed flights in the observation',
- 'arr_delay': 'Arrival delay in minutes',
- 'arr_diverted': 'Number of flights diverted',
- 'arr_flights': 'Total number of arriving flights in the observation',
- 'carrier': 'Airline carrier abbreviation',
- 'carrier_ct': 'Number of flights delayed due to air carrier (subset of 'arr_del15')',
- 'carrier_delay': 'Carrier delay in minutes (subset of arr_delay)',
- 'carrier_name': 'Airline carrier name',
- 'late_aircraft_ct': 'Number of flights delayed due to a previous flight using the same aircraft being late',
- 'late_aircraft_delay': 'Aircraft delay in minutes (subset of arr_delay)',
- 'month': 'Month (mm)',
- 'nas_ct': 'Number of flights delayed due to National Aviation System (subset 'of arr_del15)',
- 'nas_delay': 'National Aviation System in minutes (subset of arr_delay)',
- 'security_ct': 'Number of flights delayed due to airport security (subset of 'arr_del15)',
- 'security_delay': 'Security delay in minutes (subset of arr_delay)',
- 'weather_ct': 'Number of flights delayed due to weather (subset of arr_del15)',
- 'weather_delay': 'Weather delayed in minutes (subset of arr_delay)',
- 'year': 'Year (yyyy)'


## Summary of Findings

> This is a summary of my main findings:
- As the data columns are mostly numerical, I decided to use several histograms and scatterplots to emphasize the relationships between vriables. I focused mostly on plotting other variables against total flght dalays or sometimes total flights. It is worth noting that many of the numerical variables are subsets of the toal flights variable, and thus will be tied into them. Nevertheless, see the breakdown by things like delays due to late aircraft or security checks was useful to see in plotted form, especially when logarithmically transformed. This seems true for the variables that report time lost (in minutes), as well against total delay time lost.
- I plotted total delays against total flights. Not surprisingly, the correlation was positive.
- I plotted total flight delays against simlar yet unrelated categories such as cancellations and diversions. We see fewer cancellations compared to delays and even fewer diversions. I am not personally familiar with airline logistics, but it would be interesting to see if these breakdowns match the usual statistics we see in the airline industry in the United States and abroad.
- When doing box and violin plots for carrier delays, we see that all the carrier report fewerr than 500 delays for the timeframe of the dataset, although it isn't impossible to see a handful of much higher numbers. This latter spread of outliers is where we see the most variation within the carriers.
- The interesting pattern in the Total Flights histograms and other items of interest noted throughout my report can be expanded on in future investigations.
- Finally, when we plot total delay time count against all of the subcategory variables like weather, security, etc., delays to see how they compare using a plit matrix. WHen the x-axis variable is log-transformed, we see all of the variables increase as the x-axis magnitude increases. However, the first column of plots shown in the untransformed plot may be more useful, as it shows the direct breakdwon of delay subcaetegory plotted against total delays. The correlations calculated seem to confirm this finding.


## Key Insights for Presentation

> I would like to bring forward the total flights arrived vs. total delays scatterplot, the plot matrix for total delays plotted against all of the delay subcategories and the box plot for total delays by carrier. I would like to add a few details for them and touch them up to make them more asthetically pleasing and reader-fiendly.
> My goals for this explanatory data analysis:
- I think I would like to bring forward the total flights arrived vs. total delays scatterplot, the plot matrix for total delays plotted against all of the delay subcategories and the box plot for total delays by carrier. I would like to add a few details for them and touch them up to make them more asthetically pleasing and reader-fiendly.
- Specifically, I want to add jitter to the scatterplot, focus and reduce color distraction on the boxplots and add descriptive titles to the plot matrix.
- While there are many insight I would like to communicate, I wanted to communicate my findings for these three items, as they give a good sample of some of the biggest hiccups that can happen within the airline industry.

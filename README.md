## 1. Indian-States-GDP-Analysis
This is a visualization project using Python. The objective is to draw key insights from the data that can help further decision making.
We use three kind of datasets to establish a visual relation between Primary,Secondary and Tertiary Economic Sectors on Education.

## 2. Understanding the DataSet

The __first__ dataset gives us the GSDP ( Gross State Deomestic Product at Current Prices ) for a six cosecutive financial years, starting from 2011-12.<br>
The data has all Indian States in it alongwith the Growth w.r.t previous year.
There are quite a few issues with this dataset. 
- Some States Do not Have any data at all. We elimintae these entries
- Some States have some missing years.

We calculate the missing GSDP by using a straight line approximation of the previous year's data. This helps us to calculate the CAGR and Average Growth Rate
for all states. We notice that the highest GSDP States may not be the fastest growing ones.

The __second__ dataset consists of 30 separate csv files containing the contribution of various economic sectors ( Primary, Secondary and Tertiaty ) to GSDP for six years. The dataset
is not in the most friendly format. After cleaning and processing, we are able to visualize the GSDP/Capita for 2014-15 for each state and the contribution of the various sectors into the GSDP.

We now classify the states into 4 Categories C1,C2,C3 and C4 based on the GSDP/Capita ( C4 being the lowest ). The quantile values are (0.20,0.5, 0.85, 1), i.e. the states lying between the 85th and the 100th percentile are in C1, those between 50th and 85th percentile are in C2 and so on. In each category, we visualize the most prominent
sub-sectors like Manufacturing, Tourism, Agriculture etc. We can now answer these questions

- How does the GDP distribution of the top states (C1) differ from the others?
- Which sub-sectors seem to be correlated with high GDP?
- Which sub-sectors do the various categories need to focus on? 

The __third__ dataset consists of drop-out rates from primary, upper-primary, secondary, senior-secondary.

## 3. Final Objective

At this point, we have identified the fastest growing states and the key sub-sectors contributing to this.
We finally ask , if there is any correlation of GDP per capita with dropout rates in education (primary, upper primary and secondary) for the year 2014-2015 for the states.





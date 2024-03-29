# Exploratory Data Analysis & Wrangling Notes. 

## What is Data Wrangling? 

+ *Data wrangling* involves transforming raw data into formats ready for use, varying by project needs and goals. This includes merging data sources, filling or removing gaps, deleting irrelevant data, and addressing outliers for analysis.

We perform Exploratory Data Analysis to give a brief overview of the data we're working with. 

Your CSV file can be hosted online and read using the code below, creating a data frame. 
= `getURL` enables the analyst to link the file from the web. 

```{r}
read.csv(text = getURL("link")) 
```
## Reviewing the first (n) of data set rows. 
```{r}
summary(iris, 5)
tail(iris, 5) 
```

```{r}
summary(data_set$variable).
```
## If there any n/a's in your data-set, use: 
```{r}
sum(is.na(data_set))
```
+ #0 = no nulls.

### Skim
+ skim(data_set) gives a brief overview of the data.
+ You can use dplyr to group by column, then skim to get a rough idea of data distribution.

+ `filter`(data_set, price == "Ideal", table_2 > 1000)

## `mutate` 

```{r}
diamonds_new <- diamonds %>% 
  mutate(mass_g = .20 * carat) 
glimpse(diamonds_new)
```
# What is `glimpse`

+ It displays the dimensions of the dataset (number of observations and variables).
+ It shows the dataset's first few entries of each variable (column).
+ It provides the data type of each variable, such as integer, numeric, character, factor, etc.















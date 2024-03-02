# EDA

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

## Skim
+ skim(data_set) gives a brief overview of the data.
+ You can use dplyr to group by column, then skim to get a rough idea of data distribution.

#











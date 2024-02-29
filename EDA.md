# EDA

We perform Exploratory Data Analysis to give a brief overview of the data we're working with. 

Your CSV file can be hosted online and read using the below code, hence creating a data frame. 

```{r}
read.csv(text = getURL("link")) 
```
## Reviewing the first (n) of rows of the data set. 
```{r}
summary(iris, 5)
tail(iris, 5) 
```
```{r}
summary(data_set$variable).










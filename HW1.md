HW 1
================
SDS348 Spring 2021
2021-05-04

## Enter your name and EID here

**This homework is due on Feb 1, 2021 at 8am. Submit a pdf file on
Gradescope.**

*For all questions, include the R commands/functions that you used to
find your answer (show R chunk). Answers without supporting code will
not receive credit. Write full sentences to describe your findings.*

### Question 1: (2 pts)

##### The dataset `faithful` contains information about eruptions of the Old Faithful geyser in Yellowstone National Park. The first few observations are listed below.

``` r
head(faithful)
```

    ##   eruptions waiting
    ## 1     3.600      79
    ## 2     1.800      54
    ## 3     3.333      74
    ## 4     2.283      62
    ## 5     4.533      85
    ## 6     2.883      55

##### How many observations are there of each variable (i.e., how many rows are there)? What exactly do these variables measure? *Use a command to get information about the dataset.*

``` r
# your code goes here (make sure to add comments)
```

*Your answer goes here. 1-2 sentences.*

------------------------------------------------------------------------

### Question 2: (7 pts)

##### 2.1 (5 pts) What are the minimum, maximum, mean, and median values for each variable? Write sentences to describe these values. Note that there are many functions that can be used to answer this question.

``` r
# your code goes here
```

*Your answer goes here. 1-2 sentences.*

##### 2.2 (2 pts) Create a table (using - and \|) to display the statistics calculated previously for each variable.

------------------------------------------------------------------------

### Question 3: (6 pts)

##### Recall how logical indexing of a dataframe works in R. To refresh your memory, in the example code below I ask R for the number of rows in the dataset where the variable `waiting` takes on values greater than 60. Then I ask for the average of the variable `eruptions` when the variable `waiting` is above 60.

``` r
nrow(faithful[faithful$waiting>60,])
```

    ## [1] 189

``` r
mean(faithful[faithful$waiting>60,]$eruptions)
```

    ## [1] 4.138587

##### 3.1 (1 pt) What is the comma doing in the code above (i.e., why is it necessary)?

*Your answer goes here. 1-2 sentences.*

##### 3.2 (1 pt) What is the standard deviation of the variable `eruptions`?

``` r
# your code goes here
```

*Your answer goes here. 1-2 sentences.*

##### 3.3 (2 pts) What is the mean of the variable `eruptions` when `waiting` is *less than* 1 hour?

``` r
# your code goes here
```

*Your answer goes here. 1-2 sentences.*

##### 3.4 (2 pts) What is the standard deviation of the variable `eruptions` when `waiting` is *greater than* the median?

``` r
# your code goes here
```

*Your answer goes here. 1-2 sentences.*

------------------------------------------------------------------------

### Question 4: (3 pts)

##### Both variables are measured in minutes. Create two new variables named `eruptions_h` and `waiting_h` that give each variable **in hours rather than minutes** and add them to the dataset `faithful`. To help get you started, I have given you code that creates both variables but fills them with `NA` values. Replace `NA` below with code that computes the requested transformation. Print out the first few rows of the updated dataset using `head()`.

``` r
# update the code below
faithful$eruptions_h<-NA
faithful$waiting_h<-NA
```

### Question 5: (7 pts)

##### Let’s make some plots in base R.

##### 5.1 (2 pts) Create a boxplot of each variable using the `boxplot()` function and describe the distribution of each variable (e.g., use the words symmetric, skewed, the center is around \_, …). Make sure to label axes and give a title to the graph.

``` r
# your code goes here
```

*Your answer goes here. 1-2 sentences.*

##### 5.2 (2 pts) Create a histogram of each variable using the `hist()` function and describe the distribution of each variable (e.g., use the words symmetric, skewed, the center is around \_, …). Make sure to label axes and give a title to the graph.

``` r
# your code goes here
```

*Your answer goes here. 1-2 sentences.*

##### 5.3 (1 pt) Create a scatterplot by plotting both variables against each other using the `plot()` function. Make sure to label axes and give a title to the graph.

``` r
# your code goes here
```

##### 5.4 (2 pts) What can you see from the scatterplot that you cannot see from the histograms? What can you see from the histogram that you cannot see from the boxplots?

*Your answer goes here. 1-2 sentences.*

------------------------------------------------------------------------

    ##           sysname           release           version          nodename 
    ##         "Windows"          "10 x64"     "build 19041" "DESKTOP-A33VRVT" 
    ##           machine             login              user    effective_user 
    ##          "x86-64"     "Layla Guyot"     "Layla Guyot"     "Layla Guyot"

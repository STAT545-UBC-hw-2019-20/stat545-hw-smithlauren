Hw 1 Data Exploration
================
Lauren Smith
September 17, 2019

# Let’s focus on one country:

### Extract data on Germany from “Gapminder” data set

``` r
germany_data <- gapminder[c(565:576),c(3:6)]
germany_data
```

    ## # A tibble: 12 x 4
    ##     year lifeExp      pop gdpPercap
    ##    <int>   <dbl>    <int>     <dbl>
    ##  1  1952    67.5 69145952     7144.
    ##  2  1957    69.1 71019069    10188.
    ##  3  1962    70.3 73739117    12902.
    ##  4  1967    70.8 76368453    14746.
    ##  5  1972    71   78717088    18016.
    ##  6  1977    72.5 78160773    20513.
    ##  7  1982    73.8 78335266    22032.
    ##  8  1987    74.8 77718298    24639.
    ##  9  1992    76.1 80597764    26505.
    ## 10  1997    77.3 82011073    27789.
    ## 11  2002    78.7 82350671    30036.
    ## 12  2007    79.4 82400996    32170.

### Summary of Life Expectancy in Germany from 1952-2007

#### Average Life Expectancy

    ## [1] 73.44442

#### Median Life Expectancy

    ## [1] 73.15

#### Plot Germany’s life expectancy through time

``` r
attach(germany_data)
plot(year, lifeExp, xlab = "Year", ylab = "Life Expectancy", main = "Life expectancy through time")
```

![](hw1gapminderexploration_files/figure-gfm/plot%20Germany%20lifeExp%20data-1.png)<!-- -->

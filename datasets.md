* warpbreaks
  * wide to long
  * xtabs
  * warpbreaks %>% pivot_wider(names_from=c(wool),values_from=breaks,values_fn=mean)
  * reproduce that with group_by and summarise?
    * warpbreaks %>% group_by(wool,tension) %>% summarise(mean(breaks))
* relig_income
  
* gapminder
in package gapminder
  * pivot wider for year (12 levels)
* nycflights13 (package)
contains dataset `flights`
  * filter NA cases
    * flights[!complete.cases(flights),]
    * flights %>% filter(any_vars(is.na(.))) # tidyverse

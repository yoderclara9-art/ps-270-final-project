I am a current Sophmore at the University of Wisconsin-Madison majoring in Political Science with a concentration in Public Policy. For this project I am most interested in diving deeper into research related to sustainbilty application variation amoung communites as well as something related to reproductive access in the United States.


Is the gender pay gap affected by factors of one's education and one's working hours? I am using data from the IPUMS American Community Survey which supplies we with information on wages, weekly hour totals and the highest level of education one has completed. From this research, my hypothesis is that women will still earn less than men even if they work more hours or have a higher level of education. This hypothesis is based on well researched patterns in economics and sociology that women are more likely to end up in lower paying occupations and face discrimination in hiring and promotions. This usually results in lower returns to the same credentials as men. My explanatory variables are hours worked and educational attainment. My outcome variable is the wage or income measured in dollars. If the regression shows that the pay gap remains after controlling the hours and education variables, then that would support my hypothesis. If the gap disappears when these factors are added, then it would disprove my hypothesis.  

View my inital data output
---
title: "condensing data"
author: "Clara Yoder"
date: "2026-02-27"
output: html_document
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

```{r}
##   YEAR SAMPLE  SERIAL     CBSERIAL HHWT      CLUSTER GQ PERNUM PERWT SEX AGE
## 1 2024 202401  905988 2.024010e+12    9 2.024009e+12  3      1     9   2  63
## 2 2024 202401 1490438 2.024001e+12   51 2.024015e+12  1      2    97   1  32
## 3 2024 202401   61527 2.024001e+12  111 2.024001e+12  1      2    55   1  47
## 4 2024 202401 1463635 2.024000e+12   68 2.024015e+12  1      2    76   1  39
## 5 2024 202401 1253597 2.024001e+12   99 2.024013e+12  1      2   101   2  74
## 6 2024 202401 1509297 2.024000e+12   23 2.024015e+12  1      1    24   1  44
##   EDUC EDUCD UHRSWORK INCWAGE
## 1    8    81        0       0
## 2    5    50        0       0
## 3    6    63       33   45000
## 4    6    61       40       0
## 5    6    64        0       0
## 6    7    71       17   12400

gender <- readRDS("gender_wage_data_small.rds")
head(gender)

```



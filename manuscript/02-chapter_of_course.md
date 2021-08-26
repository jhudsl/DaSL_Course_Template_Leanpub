---
title: "Chapter of course"
output: html_document
---




## Learning Objectives

This chapter will cover:  

- {You can use https://www.bu.edu/cme/forms/RSS_forms/tips_for_writing_objectives.pdf to define some learning objectives here}
- {Another learning objective}

## Libraries

For this chapter, we'll need the following packages attached:


```r
library(here)
```

```
## here() starts at /home/rstudio/Desktop/GitRepos/ITCR_Course_Template_Leanpub
```

```r
library(ggplot2)
library(magrittr)
```

# Topic of Section

Text Text

## Subtopic

Text Text

### Code examples


```r
output_dir <- "code_output"
if (!dir.exists(output_dir)) {
  dir.create(output_dir)
}
```


```r
iris %>%
  ggplot(aes(Sepal.Length, Sepal.Width, color = Species)) +
  geom_point() +
  theme_bw()
```

{width: "672", align: "middle"}
![](resources/images/02-chapter_of_course_files/figure-html/unnamed-chunk-4-1.png).


```r
ggsave(file.path(output_dir, "test_ggplot2.png"))
```

```
## Saving 7 x 5 in image
```

### Image example

{alt: "Major point!! example image", width: "100%", align: "middle"}
![](resources/images/02-chapter_of_course_files/figure-html//1YmwKdIy9BeQ3EShgZhvtb3MgR8P6iDX4DfFD65W_gdQ_gcc4fbee202_0_141.png).


### Video examples


{height: "400px", width: "100%", align: "middle" type: "video" poster: "http://img.youtube.com/vi/VOCYL-FNbr0/mqdefault.jpg"}
![Click on the lower right corner to expand the screen](https://www.youtube.com/watch?v=yiZQaE0q9BY).

{height: "400px", width: "100%", align: "middle" type: "video" poster: "http://img.youtube.com/vi/VOCYL-FNbr0/mqdefault.jpg"}
![Click on the lower right corner to expand the screen](https://www.youtube.com/watch?v=VOCYL-FNbr0).

### Embedded files examples


{height: "800px", width: "672", align: "middle"}
[Check out this link](https://www.messiah.edu/download/downloads/id/921/Microaggressions_in_the_Classroom.pdf).

{height: "800px", width: "672", align: "middle"}
[Check out this link](https://widgets.figshare.com/articles/5427418/embed?show_title=1).

Example of including a website:
{height: "800px", width: "672", align: "middle"}
[Check out this link](https://yihui.org).

Example of including an html file hosted on GitHub:

{height: "800px", width: "672", align: "middle"}
[Check out this link](https://carriewright11.github.io/stringr_RLadies/index.html).


### Citation examples

We can put citations at the end of a sentence like this (Xie 2016).
Or multiple citations Xie, Allaire, and Grolemund (2018).

but they need a ; separator (Xie 2016; Xie, Allaire, and Grolemund 2018).

but they need a ; separator (\[ Xie 2016\](#bookdown2016); \[ Xie, Allaire, and Grolemund 2018\](#rmarkdown2018)).

In text, we can put citations like this Xie (2016).


Here's a silly example which may mess up references.


```r
library(oro.nifti)
```

```
## oro.nifti 0.11.0
```

```r
img <- oro.nifti::nifti()
img@.Data
```

```
## , , 1, 1
## 
##      [,1]
## [1,]    0
```

## Print out session info


```r
devtools::session_info()
```

```
## Error in get(genname, envir = envir) : object 'testthat_print' not found
```

```
## ─ Session info ───────────────────────────────────────────────────────────────
##  setting  value                       
##  version  R version 4.0.2 (2020-06-22)
##  os       Ubuntu 20.04.2 LTS          
##  system   x86_64, linux-gnu           
##  ui       X11                         
##  language (EN)                        
##  collate  en_US.UTF-8                 
##  ctype    en_US.UTF-8                 
##  tz       Etc/UTC                     
##  date     2021-08-26                  
## 
## ─ Packages ───────────────────────────────────────────────────────────────────
##  package     * version    date       lib
##  abind         1.4-5      2016-07-21 [1]
##  ari           0.4.1      2021-08-23 [1]
##  ariExtra      0.3.1      2021-08-23 [1]
##  askpass       1.1        2019-01-13 [1]
##  assertthat    0.2.1      2019-03-21 [1]
##  backports     1.1.10     2020-09-15 [1]
##  bitops        1.0-6      2013-08-17 [1]
##  bookdown      0.20       2020-06-23 [1]
##  callr         3.4.4      2020-09-07 [1]
##  cli           3.0.1      2021-07-17 [1]
##  colorspace    1.4-1      2019-03-18 [1]
##  crayon        1.4.1      2021-02-08 [1]
##  curl          4.3.2      2021-06-23 [1]
##  desc          1.2.0      2018-05-01 [1]
##  devtools      2.3.2      2020-09-18 [1]
##  digest        0.6.25     2020-02-23 [1]
##  docxtractr    0.6.5      2020-07-05 [1]
##  dplyr         1.0.2      2020-08-18 [1]
##  ellipsis      0.3.2      2021-04-29 [1]
##  evaluate      0.14       2019-05-28 [1]
##  fansi         0.5.0      2021-05-25 [1]
##  farver        2.0.3      2020-01-16 [1]
##  fs            1.5.0      2020-07-31 [1]
##  generics      0.0.2      2018-11-29 [1]
##  ggplot2     * 3.3.2      2020-06-19 [1]
##  glue          1.4.2      2020-08-27 [1]
##  gtable        0.3.0      2019-03-25 [1]
##  here        * 0.1        2017-05-28 [1]
##  highr         0.8        2019-03-20 [1]
##  hms           0.5.3      2020-01-08 [1]
##  htmltools     0.5.0      2020-06-16 [1]
##  httr          1.4.2      2020-07-20 [1]
##  jsonlite      1.7.2      2020-12-09 [1]
##  knitr         1.33       2021-08-23 [1]
##  labeling      0.3        2014-08-23 [1]
##  leanbuild     0.1.2      2021-08-23 [1]
##  lifecycle     1.0.0      2021-02-15 [1]
##  magrittr    * 2.0.1      2020-11-17 [1]
##  MASS          7.3-51.6   2020-04-26 [2]
##  memoise       1.1.0      2017-04-21 [1]
##  munsell       0.5.0      2018-06-12 [1]
##  oro.nifti   * 0.11.0     2020-09-08 [1]
##  pdftools      2.3.1      2020-05-22 [1]
##  pillar        1.6.2      2021-07-29 [1]
##  pkgbuild      1.1.0      2020-07-13 [1]
##  pkgconfig     2.0.3      2019-09-22 [1]
##  pkgload       1.1.0      2020-05-29 [1]
##  prettyunits   1.1.1      2020-01-24 [1]
##  processx      3.4.4      2020-09-03 [1]
##  progress      1.2.2      2019-05-16 [1]
##  ps            1.3.4      2020-08-11 [1]
##  purrr         0.3.4      2020-04-17 [1]
##  qpdf          1.1        2019-03-07 [1]
##  R6            2.5.1      2021-08-19 [1]
##  Rcpp          1.0.5      2020-07-06 [1]
##  remotes       2.2.0      2020-07-21 [1]
##  rlang         0.4.10     2021-08-23 [1]
##  rmarkdown     2.10       2021-08-23 [1]
##  RNifti        1.2.2      2020-09-07 [1]
##  rprojroot     1.3-2      2018-01-03 [1]
##  rstudioapi    0.11       2020-02-07 [1]
##  rvest         1.0.1      2021-07-26 [1]
##  scales        1.1.1      2020-05-11 [1]
##  sessioninfo   1.1.1      2018-11-05 [1]
##  signal        0.7-6      2015-07-30 [1]
##  stringi       1.7.3      2021-07-16 [1]
##  stringr       1.4.0      2019-02-10 [1]
##  testthat      2.3.2      2020-03-02 [1]
##  text2speech   0.3.0      2021-08-23 [1]
##  tibble        3.1.3      2021-07-23 [1]
##  tidyselect    1.1.0      2020-05-11 [1]
##  tuneR         1.3.3      2018-07-08 [1]
##  usethis       2.0.1.9000 2021-08-23 [1]
##  utf8          1.2.2      2021-07-24 [1]
##  vctrs         0.3.8      2021-04-29 [1]
##  webshot       0.5.2      2019-11-22 [1]
##  withr         2.3.0      2020-09-22 [1]
##  xfun          0.21       2021-08-23 [1]
##  xml2          1.3.2      2020-04-23 [1]
##  yaml          2.2.1      2020-02-01 [1]
##  source                                  
##  RSPM (R 4.0.3)                          
##  Github (jhudsl/ari@2638775)             
##  Github (jhudsl/ariExtra@86c733b)        
##  RSPM (R 4.0.3)                          
##  RSPM (R 4.0.3)                          
##  RSPM (R 4.0.2)                          
##  RSPM (R 4.0.3)                          
##  RSPM (R 4.0.2)                          
##  RSPM (R 4.0.2)                          
##  CRAN (R 4.0.2)                          
##  RSPM (R 4.0.0)                          
##  CRAN (R 4.0.2)                          
##  CRAN (R 4.0.2)                          
##  RSPM (R 4.0.3)                          
##  RSPM (R 4.0.3)                          
##  RSPM (R 4.0.0)                          
##  RSPM (R 4.0.2)                          
##  RSPM (R 4.0.2)                          
##  CRAN (R 4.0.2)                          
##  RSPM (R 4.0.3)                          
##  CRAN (R 4.0.2)                          
##  RSPM (R 4.0.3)                          
##  RSPM (R 4.0.3)                          
##  RSPM (R 4.0.0)                          
##  RSPM (R 4.0.1)                          
##  RSPM (R 4.0.3)                          
##  RSPM (R 4.0.3)                          
##  RSPM (R 4.0.0)                          
##  RSPM (R 4.0.3)                          
##  RSPM (R 4.0.0)                          
##  RSPM (R 4.0.1)                          
##  RSPM (R 4.0.3)                          
##  CRAN (R 4.0.2)                          
##  Github (yihui/knitr@a1052d1)            
##  RSPM (R 4.0.0)                          
##  Github (jhudsl/leanbuild@e648ebd)       
##  CRAN (R 4.0.2)                          
##  CRAN (R 4.0.2)                          
##  CRAN (R 4.0.2)                          
##  RSPM (R 4.0.0)                          
##  RSPM (R 4.0.3)                          
##  RSPM (R 4.0.2)                          
##  RSPM (R 4.0.2)                          
##  CRAN (R 4.0.2)                          
##  RSPM (R 4.0.2)                          
##  RSPM (R 4.0.3)                          
##  RSPM (R 4.0.3)                          
##  RSPM (R 4.0.3)                          
##  RSPM (R 4.0.2)                          
##  RSPM (R 4.0.3)                          
##  RSPM (R 4.0.2)                          
##  RSPM (R 4.0.3)                          
##  RSPM (R 4.0.2)                          
##  CRAN (R 4.0.2)                          
##  RSPM (R 4.0.2)                          
##  RSPM (R 4.0.3)                          
##  Github (r-lib/rlang@f0c9be5)            
##  Github (rstudio/rmarkdown@02d3c25)      
##  RSPM (R 4.0.2)                          
##  RSPM (R 4.0.0)                          
##  RSPM (R 4.0.0)                          
##  CRAN (R 4.0.2)                          
##  RSPM (R 4.0.3)                          
##  RSPM (R 4.0.3)                          
##  RSPM (R 4.0.0)                          
##  CRAN (R 4.0.2)                          
##  RSPM (R 4.0.3)                          
##  RSPM (R 4.0.0)                          
##  Github (muschellij2/text2speech@a0c9f86)
##  CRAN (R 4.0.2)                          
##  RSPM (R 4.0.3)                          
##  RSPM (R 4.0.0)                          
##  Github (r-lib/usethis@0281a15)          
##  CRAN (R 4.0.2)                          
##  CRAN (R 4.0.2)                          
##  RSPM (R 4.0.3)                          
##  RSPM (R 4.0.2)                          
##  Github (yihui/xfun@dd87cfc)             
##  RSPM (R 4.0.3)                          
##  RSPM (R 4.0.3)                          
## 
## [1] /usr/local/lib/R/site-library
## [2] /usr/local/lib/R/library
```

## References
Xie, Yihui. 2016. *Bookdown: Authoring Books and Technical Documents with R Markdown*. Boca Raton, Florida: Chapman; Hall/CRC. <https://github.com/rstudio/bookdown>.


Xie, Yihui, J. J. Allaire, and Garrett Grolemund. 2018. *R Markdown: The Definitive Guide*. Boca Raton, Florida: Chapman; Hall/CRC. <https://bookdown.org/yihui/rmarkdown>.



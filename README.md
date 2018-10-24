
<!-- README.md is generated from README.Rmd. Please edit that file -->

# plyranges-paper

The setup chunk in the [paper](paper.Rmd) shows how to download the data
with R.

The paper uses the current development version of `plyranges` which you
can install from github using:

``` r
source("https://bioconductor.org/biocLite.R")
biocLite("sa-lee/plyranges")
```

The following packages (and versions) are required to reproduce the
paper:

``` r
devtools::session_info()
#> Session info -------------------------------------------------------------
#>  setting  value                       
#>  version  R version 3.5.0 (2018-04-23)
#>  system   x86_64, darwin15.6.0        
#>  ui       X11                         
#>  language (EN)                        
#>  collate  en_AU.UTF-8                 
#>  tz       America/Los_Angeles         
#>  date     2018-06-15
#> Packages -----------------------------------------------------------------
#>  package                * version    date      
#>  acepack                  1.4.1      2016-10-29
#>  AnnotationDbi            1.42.1     2018-05-08
#>  AnnotationFilter         1.4.0      2018-05-01
#>  AnnotationHub          * 2.12.0     2018-05-01
#>  assertthat               0.2.0      2017-04-11
#>  backports                1.1.2      2017-12-13
#>  base                   * 3.5.0      2018-04-24
#>  base64enc                0.1-3      2015-07-28
#>  bindr                    0.1.1      2018-03-13
#>  bindrcpp                 0.2.2      2018-03-29
#>  Biobase                  2.40.0     2018-05-01
#>  BiocGenerics           * 0.26.0     2018-05-01
#>  BiocInstaller            1.30.0     2018-05-01
#>  BiocParallel             1.14.1     2018-05-06
#>  biomaRt                  2.36.0     2018-05-01
#>  Biostrings             * 2.48.0     2018-05-01
#>  biovizBase               1.28.0     2018-05-01
#>  bit                      1.1-13     2018-05-15
#>  bit64                    0.9-7      2017-05-08
#>  bitops                   1.0-6      2013-08-17
#>  blob                     1.1.1      2018-03-25
#>  BSgenome                 1.48.0     2018-05-01
#>  checkmate                1.8.5      2017-10-24
#>  cluster                  2.0.7-1    2018-04-13
#>  colorspace               1.3-2      2016-12-14
#>  compiler                 3.5.0      2018-04-24
#>  curl                     3.2        2018-03-28
#>  data.table               1.11.2     2018-05-08
#>  datasets               * 3.5.0      2018-04-24
#>  DBI                      1.0.0      2018-05-02
#>  DelayedArray             0.6.0      2018-05-01
#>  devtools                 1.13.5     2018-02-18
#>  dichromat                2.0-0      2013-01-24
#>  digest                   0.6.15     2018-01-28
#>  dplyr                  * 0.7.5      2018-05-19
#>  ensembldb                2.4.1      2018-05-07
#>  evaluate                 0.10.1     2017-06-24
#>  foreign                  0.8-70     2017-11-28
#>  Formula                  1.2-3      2018-05-03
#>  GenomeInfoDb           * 1.16.0     2018-05-01
#>  GenomeInfoDbData         1.1.0      2018-05-02
#>  GenomicAlignments        1.16.0     2018-05-01
#>  GenomicFeatures          1.32.0     2018-05-01
#>  GenomicRanges          * 1.32.3     2018-05-16
#>  GGally                   1.4.0      2018-05-17
#>  ggbio                  * 1.28.0     2018-05-01
#>  ggplot2                * 2.2.1.9000 2018-06-06
#>  glue                     1.2.0      2017-10-29
#>  graph                    1.58.0     2018-05-01
#>  graphics               * 3.5.0      2018-04-24
#>  grDevices              * 3.5.0      2018-04-24
#>  grid                     3.5.0      2018-04-24
#>  gridExtra                2.3        2017-09-09
#>  gtable                   0.2.0      2016-02-26
#>  Hmisc                    4.1-1      2018-01-03
#>  hms                      0.4.2      2018-03-10
#>  htmlTable                1.11.2     2018-01-20
#>  htmltools                0.3.6      2017-04-28
#>  htmlwidgets              1.2        2018-04-19
#>  httpuv                   1.4.3      2018-05-10
#>  httr                     1.3.1      2017-08-20
#>  interactiveDisplayBase   1.18.0     2018-05-01
#>  IRanges                * 2.14.10    2018-05-16
#>  knitr                  * 1.20       2018-02-20
#>  later                    0.7.2      2018-05-01
#>  lattice                  0.20-35    2017-03-25
#>  latticeExtra             0.6-28     2016-02-09
#>  lazyeval                 0.2.1      2017-10-29
#>  magrittr                 1.5        2014-11-22
#>  Matrix                   1.2-14     2018-04-13
#>  matrixStats              0.53.1     2018-02-11
#>  memoise                  1.1.0      2017-04-21
#>  methods                * 3.5.0      2018-04-24
#>  mime                     0.5        2016-07-07
#>  munsell                  0.4.3      2016-02-13
#>  nnet                     7.3-12     2016-02-02
#>  OrganismDbi              1.22.0     2018-05-01
#>  parallel               * 3.5.0      2018-04-24
#>  pillar                   1.2.2      2018-04-26
#>  pkgconfig                2.0.1      2017-03-21
#>  plyr                     1.8.4      2016-06-08
#>  plyranges              * 1.1.4      2018-05-16
#>  prettyunits              1.0.2      2015-07-13
#>  progress                 1.1.2      2016-12-14
#>  promises                 1.0.1      2018-04-13
#>  ProtGenerics             1.12.0     2018-05-01
#>  purrr                    0.2.4      2017-10-18
#>  R6                       2.2.2      2017-06-17
#>  RBGL                     1.56.0     2018-05-01
#>  RColorBrewer             1.1-2      2014-12-07
#>  Rcpp                     0.12.17    2018-05-18
#>  RCurl                    1.95-4.10  2018-01-04
#>  readr                  * 1.1.1      2017-05-16
#>  reshape                  0.8.7      2017-08-06
#>  reshape2                 1.4.3      2017-12-11
#>  rlang                    0.2.1      2018-05-30
#>  rmarkdown                1.9        2018-03-01
#>  rpart                    4.1-13     2018-02-23
#>  rprojroot                1.3-2      2018-01-03
#>  Rsamtools                1.32.0     2018-05-01
#>  RSQLite                  2.1.1      2018-05-06
#>  rstudioapi               0.7        2017-09-07
#>  rtracklayer              1.40.2     2018-05-08
#>  S4Vectors              * 0.18.2     2018-05-16
#>  scales                   0.5.0      2017-08-24
#>  shiny                    1.1.0      2018-05-17
#>  splines                  3.5.0      2018-04-24
#>  stats                  * 3.5.0      2018-04-24
#>  stats4                 * 3.5.0      2018-04-24
#>  stringi                  1.2.2      2018-05-02
#>  stringr                * 1.3.1      2018-05-10
#>  SummarizedExperiment     1.10.1     2018-05-11
#>  survival                 2.42-3     2018-04-16
#>  tibble                 * 1.4.2      2018-01-22
#>  tidyr                    0.8.1      2018-05-18
#>  tidyselect               0.2.4      2018-02-26
#>  tools                    3.5.0      2018-04-24
#>  utils                  * 3.5.0      2018-04-24
#>  VariantAnnotation        1.26.0     2018-05-01
#>  withr                    2.1.2      2018-03-15
#>  XML                      3.98-1.11  2018-04-16
#>  xtable                   1.8-2      2016-02-05
#>  XVector                * 0.20.0     2018-05-01
#>  yaml                     2.1.19     2018-05-01
#>  zlibbioc                 1.26.0     2018-05-01
#>  source                            
#>  CRAN (R 3.5.0)                    
#>  Bioconductor                      
#>  Bioconductor                      
#>  Bioconductor                      
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  local                             
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  Bioconductor                      
#>  Bioconductor                      
#>  Bioconductor                      
#>  Bioconductor                      
#>  Bioconductor                      
#>  Bioconductor                      
#>  Bioconductor                      
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  Bioconductor                      
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  local                             
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  local                             
#>  CRAN (R 3.5.0)                    
#>  Bioconductor                      
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  Bioconductor                      
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  Bioconductor                      
#>  Bioconductor                      
#>  Bioconductor                      
#>  Bioconductor                      
#>  Bioconductor                      
#>  CRAN (R 3.5.0)                    
#>  Bioconductor                      
#>  Github (tidyverse/ggplot2@4db5122)
#>  CRAN (R 3.5.0)                    
#>  Bioconductor                      
#>  local                             
#>  local                             
#>  local                             
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  Bioconductor                      
#>  Bioconductor                      
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  local                             
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  Bioconductor                      
#>  local                             
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  local (sa-lee/plyranges@ac4d090)  
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  Bioconductor                      
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  Bioconductor                      
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  Bioconductor                      
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  Bioconductor                      
#>  Bioconductor                      
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  local                             
#>  local                             
#>  local                             
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  Bioconductor                      
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  local                             
#>  local                             
#>  Bioconductor                      
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  CRAN (R 3.5.0)                    
#>  Bioconductor                      
#>  CRAN (R 3.5.0)                    
#>  Bioconductor
```


<!-- README.md is generated from README.Rmd. Please edit that file -->
plyranges-paper
===============

The setup chunk in the [paper](paper.Rmd) shows how to download the data with R.

Requires the following packages (and versions) to reproduce the paper:

``` r
devtools::session_info()
#> Session info -------------------------------------------------------------
#>  setting  value                       
#>  version  R version 3.5.0 (2018-04-23)
#>  system   x86_64, darwin15.6.0        
#>  ui       X11                         
#>  language (EN)                        
#>  collate  en_AU.UTF-8                 
#>  tz       Australia/Melbourne         
#>  date     2018-05-15
#> Packages -----------------------------------------------------------------
#>  package                * version   date       source                     
#>  acepack                  1.4.1     2016-10-29 CRAN (R 3.5.0)             
#>  AnnotationDbi            1.42.1    2018-05-08 Bioconductor               
#>  AnnotationFilter         1.4.0     2018-05-01 Bioconductor               
#>  AnnotationHub          * 2.12.0    2018-05-01 Bioconductor               
#>  assertthat               0.2.0     2017-04-11 CRAN (R 3.5.0)             
#>  backports                1.1.2     2017-12-13 CRAN (R 3.5.0)             
#>  base                   * 3.5.0     2018-04-24 local                      
#>  base64enc                0.1-3     2015-07-28 CRAN (R 3.5.0)             
#>  bindr                    0.1.1     2018-03-13 CRAN (R 3.5.0)             
#>  bindrcpp                 0.2.2     2018-03-29 CRAN (R 3.5.0)             
#>  Biobase                  2.40.0    2018-05-01 Bioconductor               
#>  BiocGenerics           * 0.26.0    2018-05-01 Bioconductor               
#>  BiocInstaller            1.30.0    2018-05-01 Bioconductor               
#>  BiocParallel             1.14.1    2018-05-06 Bioconductor               
#>  biomaRt                  2.36.0    2018-05-01 Bioconductor               
#>  Biostrings             * 2.48.0    2018-05-01 Bioconductor               
#>  biovizBase               1.28.0    2018-05-01 Bioconductor               
#>  bit                      1.1-12    2014-04-09 CRAN (R 3.5.0)             
#>  bit64                    0.9-7     2017-05-08 CRAN (R 3.5.0)             
#>  bitops                   1.0-6     2013-08-17 CRAN (R 3.5.0)             
#>  blob                     1.1.1     2018-03-25 CRAN (R 3.5.0)             
#>  BSgenome                 1.48.0    2018-05-01 Bioconductor               
#>  checkmate                1.8.5     2017-10-24 CRAN (R 3.5.0)             
#>  cluster                  2.0.7-1   2018-04-13 CRAN (R 3.5.0)             
#>  colorspace               1.3-2     2016-12-14 CRAN (R 3.5.0)             
#>  compiler                 3.5.0     2018-04-24 local                      
#>  curl                     3.2       2018-03-28 CRAN (R 3.5.0)             
#>  data.table               1.11.2    2018-05-08 CRAN (R 3.5.0)             
#>  datasets               * 3.5.0     2018-04-24 local                      
#>  DBI                      1.0.0     2018-05-02 CRAN (R 3.5.0)             
#>  DelayedArray             0.6.0     2018-05-01 Bioconductor               
#>  devtools                 1.13.5    2018-02-18 CRAN (R 3.5.0)             
#>  dichromat                2.0-0     2013-01-24 CRAN (R 3.5.0)             
#>  digest                   0.6.15    2018-01-28 CRAN (R 3.5.0)             
#>  dplyr                  * 0.7.4     2017-09-28 CRAN (R 3.5.0)             
#>  ensembldb                2.4.1     2018-05-07 Bioconductor               
#>  evaluate                 0.10.1    2017-06-24 CRAN (R 3.5.0)             
#>  foreign                  0.8-70    2017-11-28 CRAN (R 3.5.0)             
#>  Formula                  1.2-3     2018-05-03 CRAN (R 3.5.0)             
#>  GenomeInfoDb           * 1.16.0    2018-05-01 Bioconductor               
#>  GenomeInfoDbData         1.1.0     2018-05-02 Bioconductor               
#>  GenomicAlignments        1.16.0    2018-05-01 Bioconductor               
#>  GenomicFeatures          1.32.0    2018-05-01 Bioconductor               
#>  GenomicRanges          * 1.32.2    2018-05-06 Bioconductor               
#>  GGally                   1.3.2     2017-08-02 CRAN (R 3.5.0)             
#>  ggbio                  * 1.28.0    2018-05-01 Bioconductor               
#>  ggplot2                * 2.2.1     2016-12-30 CRAN (R 3.5.0)             
#>  glue                     1.2.0     2017-10-29 CRAN (R 3.5.0)             
#>  graph                    1.58.0    2018-05-01 Bioconductor               
#>  graphics               * 3.5.0     2018-04-24 local                      
#>  grDevices              * 3.5.0     2018-04-24 local                      
#>  grid                     3.5.0     2018-04-24 local                      
#>  gridExtra                2.3       2017-09-09 CRAN (R 3.5.0)             
#>  gtable                   0.2.0     2016-02-26 CRAN (R 3.5.0)             
#>  Hmisc                    4.1-1     2018-01-03 CRAN (R 3.5.0)             
#>  hms                      0.4.2     2018-03-10 CRAN (R 3.5.0)             
#>  htmlTable                1.11.2    2018-01-20 CRAN (R 3.5.0)             
#>  htmltools                0.3.6     2017-04-28 CRAN (R 3.5.0)             
#>  htmlwidgets              1.2       2018-04-19 CRAN (R 3.5.0)             
#>  httpuv                   1.4.2     2018-05-03 CRAN (R 3.5.0)             
#>  httr                     1.3.1     2017-08-20 CRAN (R 3.5.0)             
#>  interactiveDisplayBase   1.18.0    2018-05-01 Bioconductor               
#>  IRanges                * 2.14.8    2018-05-12 cran (@2.14.8)             
#>  knitr                  * 1.20      2018-02-20 CRAN (R 3.5.0)             
#>  later                    0.7.2     2018-05-01 CRAN (R 3.5.0)             
#>  lattice                  0.20-35   2017-03-25 CRAN (R 3.5.0)             
#>  latticeExtra             0.6-28    2016-02-09 CRAN (R 3.5.0)             
#>  lazyeval                 0.2.1     2017-10-29 CRAN (R 3.5.0)             
#>  magrittr                 1.5       2014-11-22 CRAN (R 3.5.0)             
#>  Matrix                   1.2-14    2018-04-13 CRAN (R 3.5.0)             
#>  matrixStats              0.53.1    2018-02-11 CRAN (R 3.5.0)             
#>  memoise                  1.1.0     2017-04-21 CRAN (R 3.5.0)             
#>  methods                * 3.5.0     2018-04-24 local                      
#>  mime                     0.5       2016-07-07 CRAN (R 3.5.0)             
#>  munsell                  0.4.3     2016-02-13 CRAN (R 3.5.0)             
#>  nnet                     7.3-12    2016-02-02 CRAN (R 3.5.0)             
#>  OrganismDbi              1.22.0    2018-05-01 Bioconductor               
#>  parallel               * 3.5.0     2018-04-24 local                      
#>  pillar                   1.2.2     2018-04-26 CRAN (R 3.5.0)             
#>  pkgconfig                2.0.1     2017-03-21 CRAN (R 3.5.0)             
#>  plyr                     1.8.4     2016-06-08 CRAN (R 3.5.0)             
#>  plyranges              * 1.1.3     2018-05-15 local (sa-lee/plyranges@NA)
#>  prettyunits              1.0.2     2015-07-13 CRAN (R 3.5.0)             
#>  progress                 1.1.2     2016-12-14 CRAN (R 3.5.0)             
#>  promises                 1.0.1     2018-04-13 CRAN (R 3.5.0)             
#>  ProtGenerics             1.12.0    2018-05-01 Bioconductor               
#>  purrr                    0.2.4     2017-10-18 CRAN (R 3.5.0)             
#>  R6                       2.2.2     2017-06-17 CRAN (R 3.5.0)             
#>  RBGL                     1.56.0    2018-05-01 Bioconductor               
#>  RColorBrewer             1.1-2     2014-12-07 CRAN (R 3.5.0)             
#>  Rcpp                     0.12.16   2018-03-13 CRAN (R 3.5.0)             
#>  RCurl                    1.95-4.10 2018-01-04 CRAN (R 3.5.0)             
#>  readr                  * 1.1.1     2017-05-16 CRAN (R 3.5.0)             
#>  reshape                  0.8.7     2017-08-06 CRAN (R 3.5.0)             
#>  reshape2                 1.4.3     2017-12-11 CRAN (R 3.5.0)             
#>  rlang                    0.2.0     2018-02-20 CRAN (R 3.5.0)             
#>  rmarkdown                1.9       2018-03-01 CRAN (R 3.5.0)             
#>  rpart                    4.1-13    2018-02-23 CRAN (R 3.5.0)             
#>  rprojroot                1.3-2     2018-01-03 CRAN (R 3.5.0)             
#>  Rsamtools                1.32.0    2018-05-01 Bioconductor               
#>  RSQLite                  2.1.1     2018-05-06 CRAN (R 3.5.0)             
#>  rstudioapi               0.7       2017-09-07 CRAN (R 3.5.0)             
#>  rtracklayer              1.40.2    2018-05-08 Bioconductor               
#>  S4Vectors              * 0.18.1    2018-05-02 Bioconductor               
#>  scales                   0.5.0     2017-08-24 CRAN (R 3.5.0)             
#>  shiny                    1.0.5     2017-08-23 CRAN (R 3.5.0)             
#>  splines                  3.5.0     2018-04-24 local                      
#>  stats                  * 3.5.0     2018-04-24 local                      
#>  stats4                 * 3.5.0     2018-04-24 local                      
#>  stringi                  1.2.2     2018-05-02 CRAN (R 3.5.0)             
#>  stringr                * 1.3.0     2018-02-19 CRAN (R 3.5.0)             
#>  SummarizedExperiment     1.10.0    2018-05-01 Bioconductor               
#>  survival                 2.42-3    2018-04-16 CRAN (R 3.5.0)             
#>  tibble                 * 1.4.2     2018-01-22 CRAN (R 3.5.0)             
#>  tidyr                    0.8.0     2018-01-29 CRAN (R 3.5.0)             
#>  tidyselect               0.2.4     2018-02-26 CRAN (R 3.5.0)             
#>  tools                    3.5.0     2018-04-24 local                      
#>  utils                  * 3.5.0     2018-04-24 local                      
#>  VariantAnnotation        1.26.0    2018-05-01 Bioconductor               
#>  withr                    2.1.2     2018-03-15 CRAN (R 3.5.0)             
#>  XML                      3.98-1.11 2018-04-16 CRAN (R 3.5.0)             
#>  xtable                   1.8-2     2016-02-05 CRAN (R 3.5.0)             
#>  XVector                * 0.20.0    2018-05-01 Bioconductor               
#>  yaml                     2.1.19    2018-05-01 CRAN (R 3.5.0)             
#>  zlibbioc                 1.26.0    2018-05-01 Bioconductor
```

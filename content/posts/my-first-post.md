---
title: "My First Post"
date: 2023-01-06T22:41:59Z
format: hugo-md
---

Hello Carl

``` r
library(tidyverse)
```

    ── Attaching packages ─────────────────────────────────────── tidyverse 1.3.2 ──
    ✔ ggplot2 3.4.0      ✔ purrr   1.0.0 
    ✔ tibble  3.1.8      ✔ dplyr   1.0.10
    ✔ tidyr   1.2.1      ✔ stringr 1.5.0 
    ✔ readr   2.1.3      ✔ forcats 0.5.2 
    ── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
    ✖ dplyr::filter() masks stats::filter()
    ✖ dplyr::lag()    masks stats::lag()

``` r
ggplot(mtcars, aes(disp, mpg)) + geom_point()
```

<img src="my-first-post.markdown_strict_files/figure-markdown_strict/unnamed-chunk-1-1.png" width="768" />

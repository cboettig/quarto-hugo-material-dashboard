---
title: "My First Post"
date: 2023-01-06T22:41:59Z
format: hugo-md
---

<script src="my-first-post_files/libs/bslib-tag-require-0.4.2/tag-require.js"></script>
<link href="my-first-post_files/libs/htmltools-fill-0.5.4/fill.css" rel="stylesheet" />


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

``` r
library(bslib)
```


    Attaching package: 'bslib'

    The following object is masked from 'package:utils':

        page

``` r
library(bsicons)
library(shiny)
library(htmltools)
card(
  card_header(
    class = "bg-dark",
    "A header"
  ),
  card_body(
    markdown("Some text with a [link](https://github.com)")
  )
)
```

<div class="card bslib-card html-fill-item html-fill-container" data-require-bs-caller="card()" data-require-bs-version="5">
<div class="card-header bg-dark">A header</div>
<div class="card-body" style="flex:0 0 auto;"><p>Some text with a <a href="https://github.com">link</a></p>
</div>
</div>

``` r
value_box(
  title = "I got", 
  value = "99 problems",
  showcase = bs_icon("music-note-beamed"),
  p("bslib ain't one", bs_icon("emoji-smile")),
  p("hit me", bs_icon("suit-spade"))
)
```

<div class="card bslib-card html-fill-item html-fill-container bslib-value-box border-0 bg-primary" data-require-bs-caller="card() value_box()" data-require-bs-version="5 5">
<div class="card-body html-fill-item html-fill-container" style="flex:1 1 auto; margin-top:auto;margin-bottom:auto; padding:0;">
<div class="bslib-column-wrap html-fill-item value-box-grid" data-require-bs-caller="layout_column_wrap()" data-require-bs-version="5" style="--bslib-column-wrap-height:auto;--bslib-column-wrap-height-mobile:auto;gap:0px; --bslib-value-box-widths:30% 70%;--bslib-value-box-widths-full-screen:1fr auto;">
<div class="html-fill-container">
<div class="html-fill-item html-fill-container">
<div class="value-box-showcase overflow-hidden html-fill-item html-fill-container" style="--bslib-value-box-max-height:100px;--bslib-value-box-max-height-full-screen:67%;"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" class="bi bi-music-note-beamed " style="height:1em;width:1em;fill:currentColor;" aria-hidden="true" role="img" ><path d="M6 13c0 1.105-1.12 2-2.5 2S1 14.105 1 13c0-1.104 1.12-2 2.5-2s2.5.896 2.5 2zm9-2c0 1.105-1.12 2-2.5 2s-2.5-.895-2.5-2 1.12-2 2.5-2 2.5.895 2.5 2z"></path>
<path fill-rule="evenodd" d="M14 11V2h1v9h-1zM6 3v10H5V3h1z"></path>
<path d="M5 2.905a1 1 0 0 1 .9-.995l8-.8a1 1 0 0 1 1.1.995V3L5 4V2.905z"></path></svg></div>
</div>
</div>
<div class="html-fill-container">
<div class="html-fill-item html-fill-container">
<div class="value-box-area html-fill-item html-fill-container border-start">
<span class="h6 mb-1">I got</span>
<span class="h2 mb-2">99 problems</span>
<p>
bslib ain't one
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" class="bi bi-emoji-smile " style="height:1em;width:1em;fill:currentColor;" aria-hidden="true" role="img" ><path d="M8 15A7 7 0 1 1 8 1a7 7 0 0 1 0 14zm0 1A8 8 0 1 0 8 0a8 8 0 0 0 0 16z"></path>
<path d="M4.285 9.567a.5.5 0 0 1 .683.183A3.498 3.498 0 0 0 8 11.5a3.498 3.498 0 0 0 3.032-1.75.5.5 0 1 1 .866.5A4.498 4.498 0 0 1 8 12.5a4.498 4.498 0 0 1-3.898-2.25.5.5 0 0 1 .183-.683zM7 6.5C7 7.328 6.552 8 6 8s-1-.672-1-1.5S5.448 5 6 5s1 .672 1 1.5zm4 0c0 .828-.448 1.5-1 1.5s-1-.672-1-1.5S9.448 5 10 5s1 .672 1 1.5z"></path></svg>
</p>
<p>
hit me
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" class="bi bi-suit-spade " style="height:1em;width:1em;fill:currentColor;" aria-hidden="true" role="img" ><path d="M8 0a.5.5 0 0 1 .429.243c1.359 2.265 2.925 3.682 4.25 4.882.096.086.19.17.282.255C14.308 6.604 15.5 7.747 15.5 9.5a4 4 0 0 1-5.406 3.746c.235.39.491.782.722 1.131.434.659-.01 1.623-.856 1.623H6.04c-.845 0-1.29-.964-.856-1.623.263-.397.51-.777.728-1.134A4 4 0 0 1 .5 9.5c0-1.753 1.192-2.896 2.539-4.12l.281-.255c1.326-1.2 2.892-2.617 4.251-4.882A.5.5 0 0 1 8 0zM3.711 6.12C2.308 7.396 1.5 8.253 1.5 9.5a3 3 0 0 0 5.275 1.956.5.5 0 0 1 .868.43c-.094.438-.33.932-.611 1.428a29.247 29.247 0 0 1-1.013 1.614.03.03 0 0 0-.005.018.074.074 0 0 0 .024.054h3.924a.074.074 0 0 0 .024-.054.03.03 0 0 0-.005-.018c-.3-.455-.658-1.005-.96-1.535-.294-.514-.57-1.064-.664-1.507a.5.5 0 0 1 .868-.43A3 3 0 0 0 14.5 9.5c0-1.247-.808-2.104-2.211-3.38L12 5.86c-1.196-1.084-2.668-2.416-4-4.424-1.332 2.008-2.804 3.34-4 4.422l-.289.261z"></path></svg>
</p>
</div>
</div>
</div>
</div>
</div>
</div>

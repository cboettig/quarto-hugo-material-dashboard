# quarto-hugo-material-dashboard
Adapting material-dashboard to Quarto and Hugo

[Demo site](https://quarto-hugo-material-dashboard.netlify.app/posts/dashboard-b/)


- HTML, CSS, JS templating from Material-Kit Dashboad (Bootstrap 5) <https://www.creative-tim.com/learning-lab/bootstrap/quick-start/material-dashboard>
- Using Hugo output format in Quarto: <https://quarto.org/docs/output-formats/hugo.html>
- ouput generated using [bslib]() and [htmltools]()

## Local Build

```bash
quarto render
hugo -c _site/content -b {baseurl}
```



## Automated deploy

- Ensure you have a gh-pages branch (e.g. check 'copy all branches' if using template repo.)
- GitHub Actions should be already configured.  This will use `quarto-dev/quarto-actions/publish@v2` (see [quarto-dev/quarto-actions](https://github.com/quarto-dev/quarto-actions)) to render the quarto files to `gh-pages` branch.
- From there, activate a Netlify deploy to hugo against the gh-pages branch to deploy the site.
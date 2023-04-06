# Data Science best practices

These are the source files for our best practice guide https://foodstandardsagency.github.io/data-science-best-practices/

The site is curated and maintained by the FSA Data Science team but we welcome feedback and contributions.

## The site

This site is built with Quarto and hosted with GitHub Pages.

The site layout and configuration is defined in `_quarto.yml`.

The site content is in the files in the `/pages` folder, which are rendered into 
HTML when the site is built and stored in the `/docs` folder. This is the folder 
that GitHub Pages reads from.

The site is automatically redeployed on any push to the main branch, with the 
`pages-build-deployment` GitHub Action.

## Contributing

If there are errors or content you would like to see, you can raise an Issue.

If you are a member of the FSA Organisation on GitHub you can make pull requests as well.

The easiest IDE for development is RStudio, which already has Quarto available (see [this guide](https://quarto.org/docs/get-started/hello/rstudio.html) to using RStudio with Quarto). You can also use [VS Code](https://quarto.org/docs/get-started/hello/vscode.html) but you will need to download Quarto first (and the Quarto extension for VS Code).

The development workflow is:

1.  Clone the repo
2.  Run `renv::restore()` to install any missing packages
3.  Create and checkout a new branch
4.  Make changes to the relevant file(s) in `/pages` and rebuild the site (Ctrl + Shift + B in Rstudio)
5.  Commit your changes and push the new branch to GitHub
6.  Open a pull request, and someone on the Data Science Team will review it

# uiucthemes 0.3.3

## CHANGES

- Handled URL changes ([#29](https://github.com/illinois-r/uiucthemes/pulls/29)) 
- Addressed CRAN feedback regarding outdated inherited documentation ([#27](https://github.com/illinois-r/uiucthemes/issues/27)) 

## DEPLOYMENT

- Updated GitHub Actions to use new versions of `R-CMD-Check` and `pkgdown`. ([#28](https://github.com/illinois-r/uiucthemes/pull/28)) 

# uiucthemes 0.3.2 (GitHub-only)

## CHANGES

- Fixed path to example images on the README page.  ([#24](https://github.com/illinois-r/uiucthemes/pulls/24)) 

## DEPLOYMENT

- Added a pkgdown website.  ([#23](https://github.com/illinois-r/uiucthemes/pulls/23)) 
- Updated GitHub Actions Runner to use tag references. ([#23](https://github.com/illinois-r/uiucthemes/pulls/23)) 

# uiucthemes 0.3.1

## CHANGES

- Fixed `citation_package = 'none'` deprecation warning by changing
  to `citation_package = 'default'` (thanks for the report [@noejn2](https://github.com/noejn2), [#21](https://github.com/illinois-r/uiucthemes/issues/21)) 
- Bumped the dependency requirements to `rmarkdown` 2.2 and `xaringan` 0.16.0.

## DOCUMENTATION

- Re-built documentation under roxygen2 7.1.0
- Modernized the README file

## DEPLOYMENT

- Switched from using TravisCI to GitHub Actions for continuous integration.

# uiucthemes 0.3.0

## NEW

- Added the `beamer_imetropolis()` template that modifies the Metropolis theme
  to match slide deck. 
    - The slides are powered by Matthias Vogelgesang's
      [`metropolis`](https://github.com/matze/mtheme), formerly "mtheme",
      for Beamer.
- Added the `html_imetropolis()` template that provides a custom illinois-themed
  Metropolis slide deck. 
    - The slides are powered by [`xaringan`](https://github.com/yihui/xaringan) 
      and Patrick Schratz's [`Metropolis` theme port](https://github.com/pat-s/xaringan-metropolis) 
      into HTML.

## CHANGES

- Added an `AUTHORS` and `COPYRIGHTS` file to describe the different templates in
  the package. 
- Improved documentation on the Beamer slide decks.
- Updated contributor email.

# uiucthemes 0.2.1

## NEW

- Added the `beamer_mil()` template for the 
  [Market Information Lab (MIL)](https://giesbusiness.illinois.edu/Margolis-Market-Information-Lab) @ UIUC
  created by [Jose Luis Rodriguez](https://giesbusiness.illinois.edu/profile/jose-luis-rodriguez-orjuela)
- Added a vignette that contains screenshots of each template.

## CHANGES

- Modified template naming scheme so that templates are grouped by "Illinois".
- Modified skeleton template of `latex_journal_format` to be more generic.

# uiucthemes 0.2.0

## NEW

- Added additional YAML header options such as licensing and safecol feature 
  to `beamer_illinois()`
- Included a preliminary version of `beamer_orange()` template created by
  [Prof. Steven Culpepper](https://stat.illinois.edu/directory/profile/sculpepp)
- Developed a template off of jss style to be used for final reports with
  [Dr. David Dalpiaz](https://daviddalpiaz.com/). 
    - This will be updated at a later point to use bookdown's `pdf_document2()` option.
- Added a non-exported helper function `load_resources_if_missing()` that
  loads any required resources into the document's working directory if they 
  are missing (e.g. `ilogo.pdf`).

## CHANGES

- UIUC recently adopted [new identity standards](https://brand.illinois.edu/). This version of `uiucthemes` applies the new guidelines in two ways:
    1. the ["Column I" logo](https://news.illinois.edu/urbana-campus-consolidates-to-single-logo/) to the ["Block I" logo](https://news.illinois.edu/urbana-campus-consolidates-to-single-logo/).
    2. Orange and Blue colors have been updated... 
        - **Orange**: `#f47f24` / `rgb(244,127,36)` to `#d75536` / `rgb(215,85,54)`
        - **Blue**: `#003c7d` / `rgb(0,60,125)` to `#1d2639` / `rgb(29,38,57)`
- Moved README images to `tools/readme` to ensure images appear on CRAN.

## DEPRECATED

- The name of the `uiuc_beamer()` theme has changed to `beamer_illinois()` as 
  a means to consistently group themes by underlying technology.

# uiucthemes 0.1.1

## NEW 

- Added `uiuc_beamer()` function that enables creation of a beamer presentation
  with UIUC colors and identity standards.
- Enabled TravisCI integration support.
- Added a `NEWS.md` file to track changes to the package.

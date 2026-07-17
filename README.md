# Concurrency Tutorial

A set of exercises that illustrate how relational concurrency does (and does not) affect the spread of HIV and other STIs. It is part of the [EpiModel](https://www.epimodel.org/) ecosystem and pairs with the interactive [concurrency.sim](https://epimodel.github.io/concurrency.sim) app.

Available at: https://epimodel.github.io/ConcurrencyTutorial

## Building locally

The site is a single [Quarto](https://quarto.org) document (`index.qmd`); figures live in `ConcurrencyTutorialFiles/`. There is no code to execute, so only Quarto is needed:

```
quarto render
```

Then open `_site/index.html`. Pushing to `main` renders and publishes to GitHub Pages via the workflow in `.github/workflows`.

## Authors

- Steven M. Goodreau, University of Washington
- Samuel M. Jenness, Emory University
- Martina Morris, University of Washington

All material is covered by a [GPL-3.0 license](https://github.com/EpiModel/ConcurrencyTutorial?tab=GPL-3.0-1-ov-file).

# Concurrency Tutorial

An interactive teaching resource on sexual partnership concurrency and how it does (and does not) shape the spread of HIV and other sexually transmitted infections. The tutorial builds intuition through a graded series of exercises, moving from simple conceptual pictures to a full stochastic network simulation, so that readers can see for themselves why concurrency matters at the population level even when it changes nothing about an individual's own risk of acquiring an infection.

It is part of the [EpiModel](https://www.epimodel.org/) ecosystem and pairs with the interactive [concurrency.sim](https://epimodel.github.io/concurrency.sim) app, which lets you explore the same simulation model without writing any code.

Available at: https://epimodel.github.io/ConcurrencyTutorial

## What the tutorial covers

The site opens with a short conceptual overview of what concurrency is (and is not) and how it drives transmission, followed by four exercises:

1. Concurrency at the local level, conceptually. Two people, sequential Sam and concurrent Chris, are given the same partners, the same sex acts, and the same timing. The exercise draws out why concurrency raises the risk to a person's partners rather than to the person practicing it.
2. Concurrency at the population level, conceptually. A small population under sequential versus concurrent partnering shows how many more people an infection can reach when partnerships overlap.
3. Concurrency at the local level, numerically. The same Sam and Chris comparison is worked out with explicit per-act transmission probabilities, making the backwards-transmission and reduced-forward-transmission effects concrete.
4. Concurrency at the population level, numerically. A full dynamic network microsimulation of an HIV epidemic that you can run and modify, turning concurrency on and off separately for women and men.

Two short appendices provide the background some readers will want: a refresher on the rules of probability, and a brief introduction to R.

## Repository layout

- `index.qmd` is the entire tutorial, authored as a single Quarto document.
- `ConcurrencyTutorialFiles/` holds the figures used throughout.
- `_quarto.yml` and `custom.scss` carry the EpiModel styling (the cosmo theme with the teal EpiModel palette and the Open Sans and Atkinson Hyperlegible fonts) along with the site navigation and footer.
- `.github/workflows/publish.yml` renders the site and publishes it to the `gh-pages` branch on every push to `main`.

## Building locally

The tutorial contains no executed code, so only [Quarto](https://quarto.org) is required; there are no R packages to install:

```
quarto render
```

Open `_site/index.html` to preview the result. To edit the content, change `index.qmd`. To change the look, edit `custom.scss` (colors and fonts) or `_quarto.yml` (navigation, table of contents, and format options). Pushing to `main` rebuilds and republishes the public site automatically.

## Authors

- Steven M. Goodreau, University of Washington
- Samuel M. Jenness, Emory University
- Martina Morris, University of Washington

See the full EpiModel team at [epimodel.org/team](https://www.epimodel.org/team.html).

## License

All material is covered by a [GPL-3.0 license](https://github.com/EpiModel/ConcurrencyTutorial?tab=GPL-3.0-1-ov-file), consistent with the EpiModel ecosystem.

# AI-Augmented Analytics for Data Visualization: Applied Exercises

Applied exercises for Erik Westlund's Yale workshop. Prompts are on the course page.

## Installation

1. Download and unzip this project, or clone this repository.
2. Install R and Quarto. Open `yale-dataviz-applied.Rproj` in RStudio, or open the folder in Positron.
3. Run `source("setup.R")` once in the R console.
4. Render a reference lesson with `quarto render docs/reference/01_data-preparation.qmd` from the project folder.
5. Open an AI assistant in this project and use the prompt from the matching module guide.

## Notebooks

| Notebook | Topic |
|---|---|
| `notebooks/style-task.qmd` | Module 3: infant mortality and income for a short report |
| `notebooks/01_data-preparation.qmd` | Module 4: inspection, filtering, recoding, and counts |
| `notebooks/02_categorical.qmd` | Module 5: counts, ordering, and proportions |
| `notebooks/03_continuous.qmd` | Module 6: distributions, outliers, quantiles, and transformations |
| `notebooks/04_group-comparison.qmd` | Module 7: grouped summaries and differences |
| `notebooks/05_association.qmd` | Module 8: scatterplots, smoothers, and model predictions |
| `notebooks/06_grab-bag.qmd` | Module 9: process diagrams and causal DAGs, if time permits |

The tasks are independent. Each notebook reads its own raw inputs. Data preparation may save a derived file in `inputs/final/` for inspection. The other tasks can run directly from the supplied raw files.

## Skills

The project includes `viz-explore`, `viz-publish`, `notebooks`, and `packages`. Their identical copies live in `.claude/skills/` and `.agents/skills/`.

## Folders

- `inputs/raw/`: PRAMS 2011, NHANES 2021–2023, Census race and ethnicity by state, country infant mortality and income, flu vaccination, and state population ranks.
- `inputs/raw/codebooks/`: dataset descriptions, variables, sources, and limitations.
- `notebooks/`: task stubs for the workshop.
- `docs/reference/`: 12 worked lessons adapted from Erik's [data visualization course](https://github.com/erikwestlund/data-visualization-2026), with project-relative paths.
- `docs/reference/ggplot2-dictionary-and-cheatsheet.qmd` and `docs/reference/dplyr-tidyr-dictionary-and-cheatsheet.qmd`: quick references for the `ggplot2`, `dplyr`, and `tidyr` functions used in the lessons.
- `outputs/`: rendered notebooks and figures. Generated files are excluded from Git.

PRAMS values are pre-aggregated percentages. Alcohol use, binge drinking, depression, and anxiety refer to the three months before pregnancy. The legacy column names contain `birth`. NHANES examples use unweighted teaching summaries. They cannot establish national estimates.

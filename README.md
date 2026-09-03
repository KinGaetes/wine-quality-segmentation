# Wine Quality Segmentation & Predictive Modeling

An interactive data-analysis project for my portfolio that explores wine quality through chemical measurements, meaningful comparisons, and transparent limitations. It prioritizes interpretation over a single global score: wine profiles are compared within analytical segments before patterns are discussed.

## Explore the project

Serve the repository locally and open `index.html` to explore the dashboard.

It includes:
- Interactive chemical-profile scatter plot with selectable axes.
- Quality distributions and top-quartile comparisons by analytical segment.
- A correlation matrix that makes within-segment relationships visible.
- A step-by-step explanation of cleaning, segmentation, and interpretation choices.
- An exploratory nearest-neighbor estimator that accepts real laboratory units rather than normalized values.
- A notebook reader that keeps the reproducible analysis connected to the portfolio.

## Why segmentation?

The original data identifies red and white wines, but chemical profiles can still differ substantially within those groups. This project uses an analytical segmentation that distinguishes non-sweet reds, non-sweet whites, and candidate sweet / late-harvest profiles. The segments are not commercial classifications; they are a way to avoid treating different chemical contexts as if they followed one universal quality rule.

The analysis deliberately treats correlation as association, not causation. For example, alcohol is consistently associated with higher scores across segments, but this does not demonstrate that increasing alcohol by itself improves a wine.

## Data
The project works from `winequality_cleaned.csv`, a cleaned and standardized version of the wine-quality data. The dashboard restores the display of chemical values to practical laboratory units, such as `% vol.`, `g/dm³`, and `mg/dm³`, while any internal distance calculation remains normalized.

Original data reference: [UCI Machine Learning Repository — Wine Quality](https://archive.ics.uci.edu/dataset/186/wine+quality).

Important limitations of the source data:

- It contains physicochemical measurements and sensory quality scores.
- It does not include origin, producer, grape variety, production method, full tasting notes, or detailed style labels.
- The estimator is exploratory and is not a replacement for tasting, cellar validation, or professional judgment.

## Author
Created by [KinGaetes](https://github.com/KinGaetes) as a data-analysis portfolio project.

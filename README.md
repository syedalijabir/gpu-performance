# Architecture Features Affecting GPU Performance
**Author:** Ali Jabir

**Date of Submission:** December 10, 2025

This project examined how GPU hardware characteristics influence its performance (TFLOP/s). Using multiple linear regression, we found strong overall model fit but unstable coefficient estimates due to severe multicollinearity among features. Ridge regression stabilized the coefficients, revealing that memory bandwidth and transistor count are the primary drivers of performance, while memory size, and thermal design power have smaller but directionally consistent effects, providing a robust and interpretable model of GPU performance scaling. The analysis is presented in a formal [`report`](paper/paper.pdf).

## Repository Structure
The repository is organized as follows:

```{bash}
gpu-performance/
├── data/
│   └── ml_hardware.csv    # cleaned data file
└── paper/
    ├── paper.qmd          # Quarto source file for the project paper
    ├── paper.pdf          # Compiled PDF of the final paper
    └── references.bib     # Bibliography file
```

## External Resources

Large Language Models (LLMs), specifically OpenAI's ChatGPT, were used as an assistant during this project. Their use was limited to the following tasks:

- Writing Assistance: Refining non-analytical sections of the report, such as the abstract and introduction. The core analytical decisions, coding, interpretation of statistical results, and final editing were performed by the author.

- BibTeX Formatting: Helping to resolve formatting issues with the bibliography file.

## Dataset
The data used in this project was sourced from [Epoch AI](https://epoch.ai/data/machine-learning-hardware).

**License:** Epoch AI's data is free to use, distribute, and reproduce provided the source and authors are credited under the [Creative Commons Attribution license](https://creativecommons.org/licenses/by/4.0/).

**Use in this Project:** This project uses the data strictly for academic and educational purposes as part of a student project. All data is attributed to its source.

## Acknowledgments
This project repository is based on the template provided by [Rohan Alexander](https://github.com/RohanAlexander/starter_folder/tree/main).

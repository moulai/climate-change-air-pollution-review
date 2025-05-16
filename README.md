# Unraveling the Complex Impact of Climate Change on Air Quality in the World

## Project Overview

Understanding how climate change affects air quality is crucial for promoting integrated environmental policy, yet current knowledge remains fragmented. In this study, we used a prompt-based large language model to systematically review over 10,000 publications, synthesizing global research patterns, mechanisms, and knowledge gaps. We found that existing research is heavily concentrated in high- and middle-income regions, while studies remain scarce in low-income countries that are more vulnerable to climate risks. Particulate matter (PM) and ozone (O₃) are the most frequently studied pollutants, with a notable shift in focus from O₃ to PM in recent years. Key climatic factors, such as temperature, wind, and humidity, affect air pollution through their influence on emissions, chemical reactions, and dispersion, with mechanisms varying across regions. Our findings underscore the urgent need for more geographically representative and mechanistically detailed research to better support coordinated air quality and climate governance, with particular attention to under-researched, high-risk regions.

This repository contains the data, code, and results associated with the paper.

## Directory Structure

The repository is organized as follows:

-   **`data/`**: Contains all data used in the study.
    -   **`raw/`**: Raw data as collected (e.g., initial literature search results). This directory will contain a `README.md` detailing the expected data and its sources.
    -   **`processed/`**: Cleaned and processed data ready for analysis (e.g., filtered document lists, extracted entities). This directory will contain a `README.md` describing the processing steps and data formats.
    -   **`supplementary/`**: Supplementary data files (e.g., expert-defined lexicons, geographical entity lists). This directory will contain a `README.md`.
-   **`src/`**: Contains all source code for the analysis.
    -   **`retrieval/`**: Scripts for literature retrieval (e.g., `retrieve_literature.py`).
    -   **`screening/`**: Scripts for document screening (e.g., `screen_documents.py`).
    -   **`information_extraction/`**: Scripts for extracting information such as CIDs, pollutants, study regions, and methods (e.g., `extract_entities.py`, `extract_methods.py`).
    -   **`systematic_review/`**: Scripts for the systematic review analyses, including research status statistical analysis and quantified synthesis of mechanisms (e.g., `analyze_research_status.py`, `synthesize_mechanisms.py`).
    -   **`visualization/`**: Scripts dedicated to generating figures presented in the paper (e.g., `plot_figure2.py`, `plot_extended_data_figure1.py`).
    -   **`utils/`**: Utility scripts containing common functions used across the project (e.g., `common_functions.py`).
-   **`notebooks/`**: Jupyter Notebooks for exploratory data analysis or specific figure generation steps (e.g., `figure_generation_exploratory.ipynb`).
    -   `figures_all_in_one.ipynb` is a notebook that contains all figure generation steps in one place and will be separated into individual codes placed in the `visualization/` directory.
    -   `figure_RADI.ipynb` is a notebook that contains the figure generation steps for the RADI analysis and will be format into a script placed in the `visualization/` directory.
-   **`docs/`**: Additional documentation, such as a link to the published paper (`paper_link.md`).
-   **`results/`**: Stores the outputs of the analyses.
    -   **`figures/`**: Generated figures from the study (initially placeholders).
    -   **`tables/`**: Generated tables from the study (initially placeholders).
-   **`README.md`**: This file, providing an overview of the project.
-   **`.gitignore`**: Specifies intentionally untracked files that Git should ignore.
-   **`LICENSE`**: The license under which this project is shared.

## Research Workflow Overview

The systematic review process followed these major stages (as depicted in Figure 1 of the paper):

1.  **Retrieval**: A combination of climate and air pollution keywords were used to perform searches, yielding over 430,000 unique search results.
2.  **Screening**: Large language models (LLMs) were used for scrutiny, and manual annotation was used for validation, narrowing down to over 10,000 relevant documents.
3.  **Information Extraction**: LLMs were combined with expert-curated keyword lists and geographical entity extraction techniques to identify article types, methods, climatic impact-drivers (CIDs), air pollutants, and research regions.
4.  **Systematic Review**: This stage was divided into two analyses:
    *   A large-scale research status statistical analysis examining temporal dynamics, spatial differences, and research attention.
    *   A quantified synthesis of mechanisms employing tailored retrieval-augmented generation (RAG) technology within a deliberately constructed mechanistic framework.

## Current Status and Future Population

**Important Note:** This repository is currently in an initial setup phase.
The directory structure and placeholder script files have been created to align with the research workflow.
**All script files (`.py`, `.ipynb`) presently contain only comments describing their intended purpose.** No runnable code is included at this stage.
Actual code, data, and results will be populated in this repository following the official publication of the paper.

## How to Navigate This Repository

-   Refer to the **Directory Structure** section above to understand where different components of the project are located.
-   The `src/` directory contains the scripts that outline the computational steps of the research.
-   The `data/` subdirectories houses the datasets used and generated. Their respective `README.md` files will offer more specific details once populated.

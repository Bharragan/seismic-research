# Automatic Classification of Volcanic Seismic
Events Using Neural Networks

[![CCDS Project Template](https://img.shields.io/badge/CCDS-Project%20template-328F97?logo=cookiecutter)](https://cookiecutter-data-science.drivendata.org/)

This repository contains all the code and resources used in the study _"Automatic Classification of Volcanic Seismic Events Using Neural Networks"_ applied to labeled seismic data from Lascar volcano, Chile.

The project applies Convolutional Neural Networks (CNNs) to spectrogram images generated from seismic waveforms for classifying five types of volcanic seismic events: Hybrid (HY), Long-Period (LP), Tectonic (TC), Tremor (TR), and Volcano-Tectonic (VT). In addition, statistical time- and frequency-domain features are extracted for exploratory data analysis.

## Key Features

- **Waveform Processing**: Tools for handling and converting seismic data (MSEED/SEISAN) using ObsPy.
- **Feature Engineering**: Extraction of time-domain and frequency-domain features.
- **Spectrogram Generation**: STFT-based spectrograms with configurable parameters.
- **Modeling**: CNN architecture in Keras/TensorFlow for image-based classification.
- **Evaluation**: Accuracy, precision, recall, F1-score, confusion matrix, and visualization.
- **Reproducibility**: Predefined structure and environment files to ensure reproducible research.

## Project Organization



```
├── LICENSE            <- Open-source license if one is chosen
├── Makefile           <- Makefile with convenience commands like `make data` or `make train`
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── external       <- Data from third party sources.
│   ├── interim        <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump.
│
├── docs               <- A default mkdocs project; see www.mkdocs.org for details
│
├── models             <- Trained and serialized models, model predictions, or model summaries
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `1.0-jqp-initial-data-exploration`.
│
├── pyproject.toml     <- Project configuration file with package metadata for 
│                         seismic_obspy and configuration for tools like black
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials.
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
├── setup.cfg          <- Configuration file for flake8
│
└── seismic_obspy   <- Source code for use in this project.
    │
    ├── __init__.py             <- Makes seismic_obspy a Python module
    │
    ├── config.py               <- Store useful variables and configuration
    │
    ├── dataset.py              <- Scripts to download or generate data
    │
    ├── features.py             <- Code to create features for modeling
    │
    ├── modeling                
    │   ├── __init__.py 
    │   ├── predict.py          <- Code to run model inference with trained models          
    │   └── train.py            <- Code to train models
    │
    └── plots.py                <- Code to create visualizations
```

--------


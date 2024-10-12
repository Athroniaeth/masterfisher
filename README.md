<div align="center">
    <h1 style="font-size: large; font-weight: bold;">Masterfisher</h1>
    <a href="#">
        <img src="https://img.shields.io/badge/Python-3.12-6">
    </a>
    <a href="#">
        <img src="https://img.shields.io/badge/License-MIT-f">
    </a>
  <br>
</div>

> ⚠️ **Warning :** Please note: this project contains neither code nor templates to protect WoW from botting, even if other solutions exist.

![img.png](docs/static/project.png)

## Presentation

This project is fishing bot for **WoW** game, fishing in a completely automatic way, mouse clicks and movements will only be done in the game and will not need any human intervention. If required, you can view what the bot is doing via a web page.

![presentation.png](docs/static/presentation.gif)

Here's the result of training on a dataset of ~200 images over 50 epochs with an imgz of 600

### Dataset analysis

Labels information (position, size and class)

![labels.jpg](docs/static/labels.jpg)

Labels histogram (correlogram)

![labels_correlogram.jpg](docs/static/labels_correlogram.jpg)

### Model training

Model training F1-confidence curve

![F1_curve.png](docs/static/F1_curve.png)

Model training precision-confidence curve

![P_curve.png](docs/static/P_curve.png)

Model training precision-recall curve

![PR_curve.png](docs/static/PR_curve.png)

Model training recall-confidence curve

![R_curve.png](docs/static/R_curve.png)

General model training results

![results.png](docs/static/results.png)

### Visualisation

Validation batch `0`

![val_batch0_labels.jpg](docs/static/val_batch0_labels.jpg)

Validation batch `1`

![val_batch1_labels.jpg](docs/static/val_batch1_labels.jpg)

## Installation

This project requires `conda` to be installed. To install the dependencies, simply run the following command:

```bash
conda env create -f environment.yml
```

You can update the environment with the following command:

```bash
conda env update -f environment.yml
```

## Usage

To run the project, you can use the following command:

```bash
python src/masterfisher/
```

## Structure

```bash
├── src               # Project source code
├── docs              # Project documentation
│   └── static        # README.md static files
├── tests             # Folder containing software tests
│   ├── units         # Unit tests
│   └── integrations  # Integration tests
├── scripts           # Useful scripts for the project (no CI/CD)
├── ruff.toml         # Ruff configuration file
├── environment.yml   # Conda environment configuration file
```

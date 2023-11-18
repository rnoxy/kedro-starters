# {{ cookiecutter.project_name }}

## Overview

This is your new Kedro project, which was generated using `kedro {{ cookiecutter.kedro_version }}`.

Take a look at the [Kedro documentation](https://docs.kedro.org) to get started.

## Rules and guidelines

In order to get the best out of the template:

* Don't remove any lines from the `.gitignore` file we provide
* Make sure your results can be reproduced by following a [data engineering convention](https://docs.kedro.org/en/stable/faq/faq.html#what-is-data-engineering-convention)
* Don't commit data to your repository
* Don't commit any credentials or your local configuration to your repository. Keep all your credentials and local configuration in `conf/local/`

## Conda environment
In order to create a conda environment based on the `conda.yml` file, run:
```bash
conda env create -f conda.yml
```
Remember to activate the conda environment in which you installed your project package before running any commands.

### direnv integration
If you have [direnv](https://direnv.net/) installed, you can automatically activate the conda environment when you `cd` into the project directory. 
```bash
# Please edit the .envrc file to fit your needs  (default conda hooks are loaded with zsh)
direnv allow # allow the .envrc file
```

## How to install project package

You can install your project package locally with:
```bash
poetry install
```
If you want to install your project package in editable mode, use:
```bash
poetry install --editable .
```

Remember that poetry will create a virtual environment for your project package, unless you are in a virtual environment already (see section about conda environment).


## How to run your Kedro pipeline

You can run your Kedro project with:

```
kedro run
```

## Project dependencies

To see and update the dependency requirements for your project use `poetry`.
For the current dependencies, see `pyproject.toml` or run `poetry show --tree`.

In order to add new dependencies for your project you will need to specify the package name and the version constraint.
For example, to add `pandas` to your project dependencies:

```
poetry add pandas@^2.0.0
```

# The `mini-poetry` Kedro starter

## Overview
This minimal [Kedro](https://kedro.org) starter sets up a lightweight Kedro project that uses the [`poetry`](https://python-poetry.org/) package manager. 


## How to use this starter
To use this starter, run:

```
kedro new --starter=https://github.com/rnoxy/kedro-starters --directory=mini-poetry --checkout v1
```

## Project structure
After creating a new project from this starter, one can find the following files and directories in the project root directory:

```
<package_name>
├── .gitignore                    - project gitignore file
├── README.md                     - project README file
├── pyproject.toml                - project metadata file
├── conf                          - project configuration directory
│   ├── base                      - directory with configuration files for all environments
│   ├── local                     - directory with configuration files for local environment
│   ├── prod                      - directory with configuration files for production environment
│   ├── test                      - directory with configuration files for test environment 
│   └── README.md                 - short explanation of configuration files
├── data                          - project data directory
│   ├── 01_raw                    - directory for raw data
│   ├── 02_intermediate           - directory for intermediate data
│   ├── 03_primary                - directory for primary data
│   ├── 04_feature                - directory for feature data
│   ├── 05_model_input            - directory for model input data
│   ├── 06_models                 - directory for models
│   ├── 07_model_output           - directory for model output data
│   └── 08_reporting              - directory for reports
├── src                           - initial project source code directory
│   └── <package_name>
│       ├── __init__.py
│       ├── __main__.py
│       ├── pipelines             - directory with pipeline's source code
│       ├── pipeline_registry.py  - pipeline registration file
│       └── settings.py           - kedro settings file
└── tests                         - directory for tests (pytest)
    ├── __init__.py
    ├── conftest.py               -  pytest configuration file
    ├── pipelines                 -  directory with pipelines tests
    └── test_run.py               -  simple example test for kedro's run
```

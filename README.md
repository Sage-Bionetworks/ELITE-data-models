# **This repository has been archived** 
*See this repo for the [current ELITE data model](https://github.com/eliteportal/data-dictionary)*

## Data Models


This repository contains 3 major files:

1. `models/EL_data_model_v3.csv`: The CSV representation of the example data model. This file is created by the collective effort of data curators and annotators from a *community* (e.g. *ELITE*), and will be used to create a JSON-LD representation of the data model.

2. `models/EL_data_model_v3.jsonld`: The JSON-LD representation of the example data model, which is automatically created from the CSV data model using the schematic CLI. More details on how to convert the CSV data model to the JSON-LD data model can be found [here](https://sage-schematic.readthedocs.io/en/develop/cli_reference.html#schematic-schema-convert). This is the central schema (data model) which will be used to power the generation of metadata manifest templates for various data types (e.g., `scRNA-seq Level 1`) from the schema.

3. `config.yml`: The schematic-compatible configuration file, which allows users to specify values for application-specific keys (e.g., path to Synapse configuration file) and project-specific keys (e.g., Synapse fileview for community project). A description of what the various keys in this file represent can be found in the [Fill in Configuration File(s)](https://sage-schematic.readthedocs.io/en/develop/README.html#fill-in-configuration-file-s) section of the schematic [docs](https://sage-schematic.readthedocs.io/en/develop/index.html).

# Requirements

Software packages installed

- Poetry - [See installation guide here](https://python-poetry.org/docs/)
- pyenv - [See guide here](https://github.com/pyenv/pyenv)

## To setup environment

After cloning the repository, run the following command:
```poetry install```

# Create a new data model
Run `scripts/convert_csv_to_json.py`

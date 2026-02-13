# LLM-4-SE
LLM for Software Engineering

This repository contains experiments and utilities for using large language models
to reason about and transform software systems as a "city of agents".

## Quick start

1. **Create and activate a virtual environment** (recommended):
   - `python -m venv .venv`
   - Windows: `.\.venv\Scripts\activate`
2. **Install dependencies**:
   - `pip install -r requirements.txt`
3. **Run an example pipeline** (from the repo root):
   - `python build_city.py`
   - or open one of the notebooks under `notebooks/` in Jupyter / VS Code.

## Project structure

- **Root Python scripts**: core utilities and pipelines for the project  
  - `build_city.py`, `build_city_buildings.py`, `build_city_research.py`, `build_city_v2.py`  
  - `clean_data.py`, `generate_simluation.py`, `universal_parser.py`  
  - Graph/feature utilities: `ast2pyg.py`, `pyg_creator.py`, `create_feature.py`, `CodeCLIP.py`, `Joern.py`

- **`notebooks/`**: interactive experimentation and demos  
  - `Experiment_1.ipynb`  
  - `demo2.ipynb`  
  - `demo6.ipynb`

- **`outputs/`**: generated artifacts and data dumps  
  - City visualizations: `city_map*.html`  
  - Simulation data: `simulation_data.csv`

- **`scripts/`**: helper shell scripts  
  - `scripts/generate_graphml.sh`

- **`requirements.txt`**: combined dependencies for data, modeling, and graph processing

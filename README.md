# geothermal_research

This repo contains the INGENIOUS dataset and the GeoDAWN dataset along with a jupyter notebooks for data exploration. There are also some setup files for running a poetry environment with instructions below. 

## Data

INGENIOUS dataset provided by the [Geothermal Data Repository (GDR)](https://gdr.openei.org/submissions/1391).
GeoDAWN dataset provided by the [USGS](https://www.sciencebase.gov/catalog/item/657e1d85d34e23d3533209f7).

## Setup

1. Install Poetry globally (skip if already installed):

**Mac/Linux:**
```bash
curl -sSL https://install.python.poetry.org | python3 -
```

**Windows (PowerShell):**
```powershell
(Invoke-WebRequest -Uri https://install.python.poetry.org -UseBasicParsing).Content | python -
```

2. Install project dependencies:
```bash
poetry install
```

3. Register the Jupyter kernel:
```bash
poetry run python -m ipykernel install --user --name=ingenious --display-name "Python (ingenious)"
```

4. Open `main.ipynb` in VS Code and select **Python (ingenious)** as the kernel.

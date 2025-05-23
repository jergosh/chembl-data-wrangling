# ChEMBL Data Wrangling

This project demonstrates querying and processing ChEMBL data to obtain a subset of hERG and CYP3A4 activity values using a Jupyter notebook.

## Requirements

- Miniconda

## Setup and execution

```bash
# Clone the repo
git clone https://github.com/jergosh/chembl-data-wrangling.git
cd chembl-data-wrangling

# Create and activate the environment
conda env create -f environment.yml

conda activate chembl-data-wrangling

# Register the kernel
python -m ipykernel install --user --name=chembl-data-wrangling --display-name "Python (chembl-data-wrangling)"

# Launch Jupyter
# jupyter lab

# OR run the notebook in the headless mode to fetch the dataset
jupyter execute notebooks/build_dataset.ipynb
```

## Output

`data/dataset.csv` -- A csv file with the following columns: chembl_id, canonical_smiles, endpoint, value (µM), pchembl.

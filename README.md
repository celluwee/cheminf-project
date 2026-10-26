# Overview
This is the final project for the Cheminformatics and Drug Design course. The idea was to take two molecular property prediction problems, one regression and one classification, and experiment with different molecular representations and model types. We started from simple classical models, improved them step by step and  tried a small graph neural network for the regression.

# Datasets

For regression we used the Lipophilicity dataset from MoleculeNet, loaded through DeepChem. It contains about 4 200 molecules from ChEMBL with measured logD values (octanol/water distribution at pH 7.4). Lipophilicity matters a lot in drug discovery because it affects solubility, membrane permeability and metabolism.

For classification we used the hERG_Karim dataset from the Therapeutics Data Commons. This dataset is a binary classification task. It has 13 445 molecules labelled as Ether-a-go-go-related gene (hERG) blockers (IC50 below 10 µM) or non-blockers, and blockers essentially represent cardiotoxic molecules.
# Setting up the environment

All notebooks except the graph neural network were run locally under Python 3.11. The environment is specified in environment.yml and can be recreated with:
```
conda env create -f environment.yml
conda activate cheminfo
pip install PyTDC==1.1.15 --no-deps
jupyter notebook
```


# Contributors
Aleksandar Krivokapić \
Olga Piskunova (aka celluwee)

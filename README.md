# GraphNetwork-Redox

Workshop materials for predicting iron-complex redox potentials with graph neural
networks. Four days of notebooks take you from the electrochemistry of Fe²⁺/Fe³⁺
through data analysis and classical ML baselines to a PyTorch Geometric GNN trained
on GPU. Built for NERSC Perlmutter, but the notebooks run anywhere.

## Setup

```bash
git clone https://github.com/fbhuiyan2/GraphNetwork-Redox.git
cd GraphNetwork-Redox
```

With `uv`:

```bash
uv venv --python 3.12.12 .uvenv
source .uvenv/bin/activate
uv pip install -r requirement.txt
```

Or with conda:

```bash
conda env create -f requirement.yaml   # creates env "mygnn"
conda activate mygnn
python -m ipykernel install --user --name fe-redox --display-name "Python (Fe-Redox)"
```

Start with `notebooks/day1-part1.ipynb`. Each notebook opens with a **Set `REPO_ROOT`**
cell that finds the repository by walking up from the notebook's directory; run it
first, and no paths need editing.

## Layout

| Path | Contents |
|---|---|
| `notebooks/` | Day 1 to 4 workshop notebooks |
| `data/` | tmQM iron-complex dataset (CSV + pickles) |
| `output/` | Everything the notebooks write: cleaned data, figures, checkpoints |
| `intro/` | Getting-started and data-handling guides |

## Notebooks

| Notebook | Topic |
|---|---|
| `day1-part1` | Environment setup, redox chemistry, why GNNs |
| `day1-part2` | Data gathering and manipulation (NumPy, pandas) |
| `day2-part1` | Exploratory data analysis, PCA, K-Means, ML basics |
| `day3` | Random Forest and GPR baselines, fingerprints, ligand analysis, molecular graphs |
| `day4` | Graph neural networks with PyTorch Geometric, cross-validation, wrap-up |

`day2-part2.ipynb`, `day5.ipynb` and `day5_advanced.ipynb` are earlier drafts kept for
reference; their content now lives in `day2-part1`, `day3` and `day4`.

## License

Creative Commons; see [LICENSE](LICENSE).

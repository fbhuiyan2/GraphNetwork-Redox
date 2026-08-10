

# Project 3
# AI, Machine Learning, and Data Science for Electrochemistry: Predicting Redox
## This project explores the intersection of AI and chemistry by using machine learning to design next-generation iron-based flow batteries.

-----

## Project Repository
* [https://github.com/alvarovm/GraphNetwork-Redox](https://github.com/alvarovm/GraphNetwork-Redox)

## AI Notebook Project

* [NotebookLM](https://notebook.google.com/notebook/214ab565-345f-4479-88a8-23d43a6fc601?authuser=1)



## Project Mentors

* Project Lead: Álvaro Vázquez-Mayagoitia
* Project Co-Lead: Fakhrul Bhuiyan
* Peer Mentor: Kareem Amin, Sophia Johnson
* Breakout Room: **D111/113**



## Project Description

Using machine learning techniques, participants will explore the role of iron complexes in advanced energy storage, specifically focusing on understanding and predicting the redox potentials that govern the performance of flow batteries. Drawing on a documented scientific workflow, participants will move through the end-to-end data science process: curating chemical datasets, analyzing molecular structures, and training Graph Neural Networks (GNNs) to make accurate physical predictions. Utilizing Python and Jupyter notebooks, students will gain practical experience in machine learning while learning how to use computational tools to address urgent challenges in sustainable energy. By the end of the program, participants will have developed a foundational understanding of how AI-enabled research methods can be applied to solve complex problems in chemistry.

## Learning Objectives

*  Explain why redox potential matters for electrochemistry, especially for iron-complex design in flow-battery applications.​
* Use Python and Jupyter notebooks to inspect, clean, organize, and visualize chemical or materials datasets.
* Distinguish between supervised learning and unsupervised learning in a scientific context.
* Understand the logic of graph-based molecular representations, where atoms are nodes and bonds are edges, as used in graph neural networks.​
* Recognize how graph neural networks can be used to connect molecular structure with chemical properties.




## GraphNetwork-Redox

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


  

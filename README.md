# The modular biochemical reaction network structure of cellular translation

Bruno Cuevas-Zuviría, Evrim Fer, Zachary R. Adam, Betül Kaçar

## Summary

This repository contains the information required to reproduce our study of translation networks

## Contents

- notebooks: simple files to run the analysis
- code: in-house library to parse and process data
- data: raw-data
- networks: results

## FAQ

**How to run things here?**


We recomend installing conda, creating a separate environment, installing pip, and installing the
library at the *code* folder.

	conda env create --file environment.yml
	cd code
	pip install -e $(pwd)


To run the Node2Vec analysis, you will need a working version of PyTorch loaded in your environment.
Given that PyTorch installation depends on your hardware (e.g. GPU, cpu; MacOS, Linux), we recommend to 
access the [PyTorch]() webpage to find detailed instructions.

If you don't have a GPU, it's likely that the following lines will just make it work:

	conda install pytorch==1.12.0 cpuonly -c pytorch # PyTorch 1.12 for gpu
	conda install pyg -c pyg # PyTorch Geometric


For technical queries, contact cuevaszuviri@wisc.edu

# Setup Instructions same as repo provide deadme file

## Clone Repository

git clone https://github.com/oxpig/LICHEN.git

## Create Environment

conda create -n LICHEN_env python=3.10

conda activate LICHEN_env

## Install Dependencies

conda install -c conda-forge biopython

conda install -c conda-forge pytorch

conda install -c conda-forge anarcii

pip install ablang2

pip install .

## Download Weights

Download from Zenodo:

https://doi.org/10.5281/zenodo.15917096

Place file:

model/model_weights.pt

## Test

from lichen import LICHEN

model = LICHEN("model/model_weights.pt")

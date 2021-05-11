# CMSC740Project
Code for cmsc740project

This repo contains the code for ablation studies for the [paper](https://arxiv.org/abs/2002.10099), [original repo](https://github.com/amosgropp/IGR).

Requirements:
* Python 3.7 or later
* Pytorch 1.2 or later
* Numpy, pycohon, plotly, scikit-image, trimesh

Original paper results for surface reconstruction:

In reconstruction/setup.conf, in train, change the input_path to path of the corresponding input .ply file on your local machine.
Then for training, run python reconstruction/run.py.

Ablation studies:
* For changing the weightage of the second loss term, in reconstruction/setup.conf, change the value of lambda in network/loss key.
* For changing the skip connection, in reconstruction/setup.conf, change the field skip_in in network.inputs.

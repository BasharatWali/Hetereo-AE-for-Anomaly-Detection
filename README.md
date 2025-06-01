# Hetereo-AE-for-Anomaly-Detection

Project Overview

This repository contains a Jupyter notebook that implements and evaluates a Heterogeneous Autoencoder (Hetero‐AE) for unsupervised anomaly detection in brain MRI scans. The key components include:

    Data Preprocessing

        Brain extraction (skull‐stripping) and intensity normalization

        Resizing and 2D‐slice extraction from IXI (healthy) and BraTS‐21 (tumour) datasets

    Model Implementation

        ResNet-34–based CNN encoder

        Hybrid CNN–Transformer decoder with Multi-Scale Sparse Transformer Blocks (MSTBs)

        Multi-stage feature comparison loss combining MSE and cosine similarity

    Training & Evaluation

        Trains on healthy IXI slices with on-the-fly augmentations (flips, rotations, intensity jitter)

        Tests on skull-stripped BraTS-21 slices and generates anomaly heatmaps

    Visualizations

        Example anomaly maps overlaid on BraTS-21 inputs to highlight tumour regions

        Training loss curves and feature discrepancy plots

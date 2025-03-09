# Ionization Energy Prediction Using SchNet

## Overview
This project aims to predict the ionization energy of molecules using a neural network model, specifically SchNet, which is designed for molecular property predictions. The model is trained on the **QM9 dataset**, which includes various molecular properties. Ionization energy is derived from the **Highest Occupied Molecular Orbital (HOMO)** energy, as the ionization energy is typically defined as the negative value of HOMO.

The code in this repository is a reimplementation and retraining of the SchNet model using the QM9 dataset. The model takes molecular structural information (e.g., atomic numbers, positions) and predicts the ionization energy, which can be used for further molecular design or understanding material properties.

## Project Structure
- **Model**: Implements the SchNet architecture, which uses atomistic representations for molecular property prediction.
- **Dataset**: The QM9 dataset is used, which includes properties like HOMO, LUMO, and ionization energies.
- **Training**: The model is trained using the ionization energy as the target property, derived from HOMO values in the dataset.
- **Results**: Ionization energies are predicted for molecules like H₂O and K₂O, with the results compared and analyzed.
  
## Requirements
- Python 3.6 or higher
- PyTorch 1.9+
- SchNetPack
- ASE (Atomic Simulation Environment)
  
You can install the required dependencies using pip:

```bash
pip install torch schnetpack ase

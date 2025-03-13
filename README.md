# GAN-Based Music Style Transfer using MIDI Chroma and Pix2Pix
A GAN-based model that learns to modify musical texture while preserving harmonic structure using pix2pix and MIDI chroma features.


## Overview
This project explores **music style transfer** using **Generative Adversarial Networks (GANs)**, specifically a **pix2pix model**. The goal is to modify the **musical texture** of a piece while maintaining its harmonic structure.

The model learns to **map chroma features from MIDI data** to musical textures, similar to how **pix2pix** performs image-to-image translation.

The project is divided into three main parts:
- **Extracting chroma features from MIDI data.**
- **Training a pix2pix model** to learn musical texture transformations.
- **Generating transformed MIDI sequences** with new textures.

## Dataset
The project works with **MIDI files**, extracting chroma features as input for the GAN-based model.

## Project Structure
### Data Preprocessing
- Loads and processes **MIDI data**.
- Extracts **chroma features** to represent harmonic structure.
- Converts MIDI textures into a suitable format for training.

### GAN-Based Model Implementation
- Implements a **pix2pix model** for style transfer.
- Uses a **U-Net-based generator** to predict musical textures.
- Trains with an **adversarial loss function**.

### Evaluation & Results
- Generates MIDI sequences with transformed textures.
- Compares input vs. output MIDI files.
- Visualizes chroma features before and after transformation.

## Installation & Requirements
To run this notebook, you need **Python 3** and the following dependencies:

```sh
pip install torch torchvision numpy librosa pretty_midi
```

## Usage
Clone the repository:

```sh
git clone https://github.com/LidanAvisar/GAN-Based-Music-Style-Transfer-using-MIDI-Chroma-and-Pix2Pix
cd GAN-Based-Music-Style-Transfer-using-MIDI-Chroma-and-Pix2Pix
```

Open the Jupyter Notebook:

```sh
jupyter notebook "GAN_Music_Style_Transfer.ipynb"
```

Run all cells to train and evaluate the model.

## Results & Analysis
The notebook visualizes:
- **Original vs. transformed MIDI chroma features.**
- **Generated MIDI sequences.**
- **Training loss curves for the GAN model.**

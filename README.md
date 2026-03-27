# Mikayla Subgraph Script

Analysis and visualization of NbCrVWZr high-entropy alloy composition space using UMAP and graph-based methods.

## Overview

This project analyzes a dataset of NbCrVWZr (Niobium-Chromium-Vanadium-Tungsten-Zirconium) alloy compositions and their materials properties. The analysis includes:

- **UMAP Visualization**: 2D embeddings of alloy compositions colored by elemental composition and material properties
- **Graph Database Analysis**: Construction of composition neighbor graphs and identification of connected components
- **Property Analysis**: Filtering and analysis of material properties including:
  - Solidification range
  - BCC (Body-Centered Cubic) phase stability at multiple temperatures
  - Yield strength at 1000°C
  - Creep resistance
  - Pugh ratio (ductility indicator)
  - Kou criteria

## Files

- `NbCrVWZr Graph Database Analysis.ipynb` - Main Jupyter notebook with all analysis
- `NbCrVWZr_dataset_1.xlsx` - Materials dataset with compositions and properties
- `nimplex_GF_5_20_nodes.npy` - NumPy array of node characteristics
- `nimplex_GF_5_20_neighbors.npy` - NumPy array of neighbor relationships

## Dependencies

Install dependencies using:

```bash
pip install -r requirements.txt
```

Key libraries:
- `numpy` - Numerical computations
- `pandas` - Data manipulation
- `networkx` - Graph analysis
- `matplotlib` - Visualization
- `seaborn` - Statistical visualization
- `openpyxl` - Excel file handling
- `Pillow` - Image processing

## Usage

1. Install dependencies: `pip install -r requirements.txt`
2. Open the notebook: `jupyter notebook "NbCrVWZr Graph Database Analysis.ipynb"`
3. Run cells sequentially to generate visualizations and analysis

## Key Analyses

### 1. Component Identification
The notebook identifies connected components in the alloy composition space based on BCC stability criteria, revealing distinct regions of material property space.

### 2. Property Distributions
KDE plots and radar plots show property distributions across connected components, enabling comparison of different compositional regions.

### 3. Filtering Criteria
- **Solidification Range**: Compositions with solidification range ≤ 50 K
- **BCC Stability**: Compositions with BCC phase fraction ≥ 0.999 at various temperatures
- **Scheil Analysis**: Non-equilibrium solidification analysis

## Output

The notebook generates:
- PNG visualizations of UMAP embeddings
- Excel files with component statistics
- Radar plots for multi-property comparison
- Combined radar plot visualization

## Citation

If using this analysis in research, please cite the original dataset and describe the filter criteria applied.

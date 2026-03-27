# Setup Guide for CGA_Subgraph_Analysis

## Quick Start
To get started quickly with CGA_Subgraph_Analysis, follow the steps outlined below:

1. Clone the repository:
   ```bash
   git clone https://github.com/jameshanagan/CGA_Subgraph_Analysis.git
   cd CGA_Subgraph_Analysis
   ```
2. Install the necessary dependencies (as outlined in the installation instructions below).
3. Make sure you have the required data files in place.
4. Execute the provided Jupyter notebooks to analyze the subgraph data.

## Installation Instructions
You can install the necessary packages using either pip or conda.

### Using pip
Run the following command:
```bash
pip install -r requirements.txt
```

### Using conda
You can also create a conda environment with the following command:
```bash
conda create --name cga_env python=3.8
conda activate cga_env
conda install --file requirements.txt
```

## Data Files Documentation
- The data files required for the analysis can be found in the `data/` directory.
- Make sure to review the file names and formats to ensure compatibility with the analysis scripts.

## Notebook Structure
- The project contains several Jupyter notebooks, each designed for specific parts of the analysis:
  - `intro_to_analysis.ipynb`: Introduction and overview.
  - `data_preprocessing.ipynb`: Data cleaning and preparation.
  - `analysis.ipynb`: Primary analysis scripts.
  - `visualization.ipynb`: Visualizing the results.

## Troubleshooting
In case of any issues during installation or execution, consider the following steps:
- Ensure all dependencies are correctly installed.
- Check the compatibility of data files with the scripts.
- Review the error messages for hints on what went wrong.

## Performance Notes
- Performance may vary based on your machine configuration. For optimal performance, ensure that you have sufficient memory and processing power available.
- If you encounter slow performance, consider limiting the size of the input data or optimizing the analysis scripts.

Happy analyzing!
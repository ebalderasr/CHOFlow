# Red/Green Ratio Analysis for CHO Clones b and c

This project focuses on analyzing the red/green fluorescence ratio (`BL2-A` / `BL1-A`) for CHO cell clones `b` and `c` over multiple time points. It provides tools to filter data, compute the ratio, visualize distributions, and perform statistical comparisons between clones.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [License](#license)

## Overview

CHO cells are widely used for protein production in biotechnology. This analysis focuses on understanding fluorescence emission ratios to evaluate mitochondrial activity or other relevant characteristics between two CHO clones (`b` and `c`).

## Features

- **Data Filtering**:
  - Focuses only on clones `b` and `c` for the analysis.
- **Ratio Calculation**:
  - Computes the red/green ratio (`BL2-A` / `BL1-A`) for each event in the dataset.
- **Visualization**:
  - Generates violin plots to visualize the ratio distributions across clones and time points.
- **Statistical Analysis**:
  - Performs Student's t-test and Mann-Whitney U test to compare clones at each time point.
- **Result Summary**:
  - Outputs a table with statistical results for all time points.

## Installation

To run this script, ensure you have Python 3.7+ installed along with the following libraries:

```bash
pip install numpy pandas seaborn matplotlib scipy
```

## Usage

1. **Prepare Your Data**:
   - The dataset should include these columns:
     - `BL1-A`: Green fluorescence emission.
     - `BL2-A`: Red fluorescence emission.
     - `Clone`: Clone identifiers (`b` and `c`).
     - `Time`: Time points for the experiment.

2. **Run the Script**:
   - Execute the script in your Python environment:
     ```bash
     python Red_Green_Ratio_Analysis.py
     ```

3. **Outputs**:
   - Violin plots for the red/green ratio distributions.
   - A summary table with statistical results for clones `b` and `c` at each time point.

## Results

- **Visualizations**:
  - Violin plots provide an overview of the distribution of red/green ratios by clone and time.
- **Statistical Tests**:
  - Outputs include:
    - T-statistic and p-value from Student's t-test.
    - U-statistic and p-value from Mann-Whitney U test.

## Example Outputs

### Violin Plot
A violin plot visualizing the red/green ratio distributions for clones `b` and `c` across time points.

### Statistical Summary
| Time | T-Statistic | P-Value T-Test | U-Statistic | P-Value Mann-Whitney U |
|------|-------------|----------------|-------------|------------------------|
| 1    | 2.53        | 0.013          | 125.0       | 0.010                 |

## Authors

**Emiliano Balderas Ramírez**  
PhD Student at the Instituto de Biotecnología, UNAM  
Email: ebalderas@live.com.mx  
Phone: +52 2221075693  

**Dr. Octavio Tonatiuh Ramírez Reivich**  
Principal Investigator, Instituto de Biotecnología, UNAM  
Email: tonatiuh.ramirez@ibt.unam.mx  

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For questions or suggestions, feel free to contact:  

**Emiliano Balderas Ramírez**  
PhD Student at the Instituto de Biotecnología, UNAM  
Email: ebalderas@live.com.mx  
Phone: +52 2221075693
``` 
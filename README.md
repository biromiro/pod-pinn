# Burgers' Physics-Informed Surrogate leveraging Proper Orthogonal Decomposition

## Overview

This repository contains the implementation of a physics-informed surrogate model that leverages Proper Orthogonal Decomposition (POD) and neural networks to efficiently solve the inviscid Burgers' equation. This project integrates the dimensionality reduction capabilities of POD with the predictive power of neural networks, incorporating Physics-Informed Neural Networks (PINNs) principles to ensure physical consistency in the solutions.

## Repository Structure

```
├── src
│   ├── dl_roms_clean.ipynb
│   ├── plots.ipynb
│   ├── requirements.txt
├── docs
│   ├── naml-report.pdf
│   ├── naml-present.pdf
├── README.md
```

- **src/**: Contains the source code and notebooks for model implementation and analysis.
  - `dl_roms_clean.ipynb`: Notebook for training and evaluating the POD-NN model.
  - `plots.ipynb`: Notebook for generating plots and visualizations related to the project.
  - `requirements.txt`: Python libraries required to run the notebooks.
  
- **docs/**: Contains the documentation and reports related to the project.
  - `naml-report.pdf`: Detailed project report.
  - `naml-present.pdf`: Project presentation slides.

## Getting Started

### Prerequisites

Ensure you have the following dependencies installed:
- Python 3.10
- Jupyter Notebook
- Libraries: [dlroms](https://github.com/NicolaRFranco/dlroms/tree/main), jax, matplotlib, numpy, [phiflow](https://github.com/tum-pbs/PhiFlow), pytorch

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/burgers-pinn-pod.git
   cd burgers-pinn-pod
   ```

2. Install the required Python packages:
   ```bash
   pip install -r src/requirements.txt
   ```

### Running the Notebooks

1. Navigate to the `src` directory:
   ```bash
   cd src
   ```

2. Open and run the `dl_roms_clean.ipynb` notebook to train and evaluate the POD-NN model:
   ```bash
   jupyter notebook dl_roms_clean.ipynb
   ```

3. Open and run the `plots.ipynb` notebook to generate the relevant plots and visualizations:
   ```bash
   jupyter notebook plots.ipynb
   ```

## Project Description

The goal of this project is to create a surrogate model that combines Proper Orthogonal Decomposition (POD) with neural networks to reduce the computational complexity of solving the inviscid Burgers' equation. By incorporating Physics-Informed Neural Networks (PINNs), the model ensures that the predictions adhere to the underlying physical laws.

### Key Features

- **Proper Orthogonal Decomposition (POD):** Reduces the dimensionality of the system while preserving its most significant features.
- **POD-NN Hybrid Model:** Combines POD with neural networks to map new parameters to POD coefficients for efficient state prediction.
- **Physics-Informed Neural Networks (PINNs):** Incorporates physical laws directly into the neural network architecture, ensuring the predictions adhere to known physical principles.
- **Efficient Data Generation:** Utilizes high-fidelity data generation frameworks for robust model training.
- **Multiple Training Regimes:** Evaluates supervised, unsupervised, and mixed training methods to balance accuracy and physical fidelity.

### Results

The results of the project demonstrate the effectiveness of integrating POD with PINNs, showing improved computational efficiency and adherence to physical laws compared to traditional methods. Detailed results and analysis can be found in the `naml-report.pdf` in the `docs` folder.

## Documentation

For a detailed explanation of the methodology, experiments, and results, refer to the following documents in the `docs` folder:
- `naml-report.pdf`: Detailed project report.
- `naml-present.pdf`: Project presentation slides.

## Acknowledgements

This project was developed as part of the Numerical Analysis for Machine Learning course at Politecnico di Milano, Italy. Special thanks to [Dr. Nicola Rares Franco](https://github.com/NicolaRFranco) for his invaluable support and guidance.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

If you have any questions or need further assistance, please feel free to contact me at [n.r.t.c@hotmail.com](n.r.t.c@hotmail.com).

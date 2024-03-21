# Reconstructing Rotation Curves with Neural Networks

This repository presents a novel approach to reconstructing galaxy rotation curves using neural networks, specifically leveraging the capabilities of Genetic Algorithms for parameter optimization. Our methodology employs the DEAP library with our custom ([NNOGADA code](https://github.com/igomezv/Nnogada)) for efficient and effective tuning of neural network parameters.

## Overview

Galaxy rotation curves are critical for understanding the mass distribution within galaxies. Traditional methods of analyzing these curves often involve extensive manual effort and subjective judgment. Our project introduces a machine-learning-based approach to automate and enhance the accuracy of rotation curve reconstruction.

## Repository Contents

- **models**: This directory contains binary `.h5` files of all the neural network models we have trained. These models are ready to use for predicting galaxy rotation curves.
  
- **figures**: Here, you'll find various plots related to the reconstruction of rotation curves and the visualization of loss functions over the training period. These figures illustrate the effectiveness and convergence of our models.

- **data**: This directory hosts the original observational data of rotational curves from the THINGS survey, kindly provided by Prof. Erwing De Blok.
  
  ### Data References
  - Carlos R. Argüelles and Santiago Collazo. "Galaxy rotation curve fitting using machine learning tools." *Universe*, 9(8):372, 2023.
  - Connor J. Stone, Nikhil Arora, Stéphane Courteau, and Jean-Charles Cuillandre. "Autoprof–I. An automated non-parametric light profile pipeline for modern galaxy surveys." *Monthly Notices of the Royal Astronomical Society*, 508(2):1870–1887, 2021.

## How to Use

1. **Setting Up**: Clone this repository to your local machine. Ensure you have Python and the necessary libraries installed.
2. **Running Models**: Navigate to the `models` directory. Use the provided scripts to load and run predictions using our pre-trained neural networks.
3. **Visualization**: To view the reconstruction plots and loss functions, head to the `figures` directory. Additional scripts are available for generating new plots.

## Contributing

We welcome contributions from the community. If you'd like to improve the models, suggest new features, or report issues, please feel free to open an issue or submit a pull request.

## Acknowledgments

We extend our gratitude to Prof. Erwing De Blok for providing the rotational curve data from the THINGS survey.


## Citation

If you use this work in your research, please cite:

```bibtex
@article{RCneural,
  title={Reconstructing Rotation Curves with Neural Networks},
  author={Garcia-Arroyo, G. and Gomez-Vargas, I. and Vazques, JA.},
  journal={ArXiV:xxxxx},
  year={2024},
  volume={},
  pages={}
}

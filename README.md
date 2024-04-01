# Reconstructing Rotation Curves with Neural Networks

This repository presents a novel approach to reconstructing galaxy rotation curves using neural networks optimized with genetic algorithms. Our methodology employs the DEAP library with our [`nnogada` framework](https://github.com/igomezv/Nnogada) for efficient and effective tuning of neural network hyperparameters.

## Overview

Galaxy rotation curves are critical for understanding the mass distribution within galaxies. Traditional methods of analyzing these curves often involve extensive manual effort. Our project introduces a machine-learning approach to generate rotation curve reconstructions based on the observational data.

## Repository Contents

- **models**: This directory contains binary `.h5` files of all the neural network models we have trained. These models are ready to use for predicting galaxy rotation curves.
  
- **figures**: Here, you'll find various plots related to the reconstruction of rotation curves and the visualization of loss functions over the training period. These figures illustrate the effectiveness and convergence of our models.

- **data**: This directory hosts the original observational data of rotational curves from the THINGS survey, kindly provided by Prof. Erwing De Blok.
  
  ### Data References
  - Walter, F., Brinks, E., De Blok, W. J. G., Bigiel, F., Kennicutt, R. C., Thornley, M. D., & Leroy, A. (2008). THINGS: The H i nearby galaxy survey. The Astronomical Journal, 136(6), 2563.
  - De Blok, W. J. G., Walter, F., Brinks, E., Trachternach, C., Oh, S. H., & Kennicutt, R. C. (2008). High-resolution rotation curves and galaxy mass models from THINGS. The Astronomical Journal, 136(6), 2648.

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
  author={Garcia-Arroyo, G. and Gomez-Vargas, I. and Vazquez, JA.},
  journal={ArXiV:xxxxx},
  year={2024},
  volume={},
  pages={}
}
```

If you find useful our `nnogada` framework:

```bibtex
@article{nnogada,
  title={Neural networks optimized by genetic algorithms in cosmology},
  author={Gómez-Vargas, I. and Andrade, J. B. and Vázquez, J. A.},
  journal={Physical Review D},
  volume={107},
  number={4},
  pages={043509},
  year={2023},
  publisher={American Physical Society},
  doi={https://doi.org/10.1103/PhysRevD.107.043509},
  url={https://doi.org/10.48550/arXiv.2209.02685}
}
```

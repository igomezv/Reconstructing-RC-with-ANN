<a href="https://arxiv.org/abs/2404.05833">
  <img src="https://img.shields.io/badge/arXiv-2404.05833-b31b1b.svg" alt="arXiv:2404.05833">
</a>

# Reconstructing Rotation Curves with Neural Networks

This repository presents a novel approach to reconstructing galaxy rotation curves using neural networks optimized with genetic algorithms. Our methodology employs the DEAP library with our [`nnogada`](https://github.com/igomezv/Nnogada) framework for efficient and effective tuning of neural network hyperparameters.

## Overview

Galaxy rotation curves are critical for understanding the mass distribution within galaxies. Traditional methods of analyzing these curves often involve extensive manual effort. Our project introduces a machine-learning approach to generate rotation curve reconstructions based on the observational data.

## How to Use

1. **Setting Up**: Clone this repository to your local machine. Ensure you have Python and the necessary libraries installed.
    - You can use the .yml file to recreate the anaconda environment:
      
        - ``conda env create -f environment.yml``
        
    - Otherwise, we recommend the following to avoid incompatibilities in some libraries:
        - ``conda create -n neuralrcenv python=3.8``
        - ``conda activate neuralrcenv``
        -  ``conda install numpy seaborn matplotlib scikit-learn tensorflow==2.12``
        -  ``pip install astroNN``.

    - Finally, if you want to retrain the neural network models with genetic algorithms, please clone or download `nnogada` from [here](https://github.com/igomezv/Nnogada).

3. **Running Models**: Navigate to the `models` directory. Use the provided scripts to load and run predictions using our pre-trained neural networks.
4. **Visualization**: To view the reconstruction plots and loss functions, head to the `figures` directory. Additional scripts are available for generating new plots.



## Repository Contents

- **ALL_RC_mass_models.ipynb** contains the hyperparameter tuning for all the galaxies using `nnogada`. **load_all_models.ipynb** allows to load the `.h5` saved models, trained in the **ALL_RC_mass_models.ipynb** notebook. **RC_neural_model.ipynb** and **RC_mass_models.ipynb** notebooks have preliminary/exploratory tests.

- **models/**: This directory contains binary `.h5` files of all the neural network models we have trained. These models are ready to use for predicting galaxy rotation curves.
  
- **figures/**: Here, you'll find various plots related to the reconstruction of rotation curves and the visualization of loss functions over the training period. These figures illustrate the effectiveness and convergence of our models.

- **data/**: This directory hosts the original observational data of rotational curves from the THINGS survey, kindly provided by Prof. Erwing De Blok.
  
  ### Data References
  - Walter, F., Brinks, E., De Blok, W. J. G., Bigiel, F., Kennicutt, R. C., Thornley, M. D., & Leroy, A. (2008). THINGS: The H i nearby galaxy survey. The Astronomical Journal, 136(6), 2563.
  - De Blok, W. J. G., Walter, F., Brinks, E., Trachternach, C., Oh, S. H., & Kennicutt, R. C. (2008). High-resolution rotation curves and galaxy mass models from THINGS. The Astronomical Journal, 136(6), 2648.


## Contributing

We welcome contributions from the community. If you'd like to improve the models, suggest new features, or report issues, please feel free to open an issue or submit a pull request.

## Acknowledgments

We extend our gratitude to Prof. Erwing De Blok for providing the rotational curve data from the THINGS survey.


## Citation

If you use this work in your research, please cite:

```bibtex
@article{RCneural,
  title={Reconstructing Rotation Curves with Neural Networks},
  author={Garcia-Arroyo, G. and Gómez-Vargas, I. and Vázquez, J. A.},
  journal={ArXiV:xxxxx},
  year={2024},
  volume={},
  pages={}
}
```

If you find useful our [`nnogada`](https://github.com/igomezv/Nnogada) framework:

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

- Method for reconstructions with neural networks:
```bibtex
@article{gomez2023neural,
  title={Neural network reconstructions for the Hubble parameter, growth rate and distance modulus},
  author={G{\'o}mez-Vargas, Isidro and Medel-Esquivel, Ricardo and Garc{\'\i}a-Salcedo, Ricardo and V{\'a}zquez, J Alberto},
  journal={The European Physical Journal C},
  volume={83},
  number={4},
  pages={304},
  year={2023},
  publisher={Springer}
}
```

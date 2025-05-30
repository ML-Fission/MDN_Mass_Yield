# MDN_Mass_Yields
Mixture Density Network for neutron induced fission mass yields

### In requirements.txt are the required libraries: 
```pip install -r requirements.txt```

## Data 

**Training Data** -> Samples from Gaussian Process Regression or Gaussian Mixture Regression
or 
**Training Data** -> Samples from JENDL data
or
**Training Data** -> Samples from Gaussian Process Regression w/ WhiteKernel

**Test Data** -> Experimental data from JENDL 4.0
or
**Test Data** -> Split Experimental data

## Mixture Density Network Structure (GPR | GMR Sampling for training)

### Layers

- **9** Hidden **relu** layers
- **1** Hidden **tanh** layer for smoothness
- Mixture Density layer (output)

### Neurons
**100** neurons/layer

### Number of mixes (Gaussians)
**3** mixes

## Mixture Density Network Structure (JENDL data training)

### Layers

- **9** Hidden **relu** layers
- **1** Hidden **tanh** layer for smoothness
- Mixture Density layer (output)

### Neurons
**100** neurons/layer

### Number of mixes (Gaussians)
**3** mixes

## Mixture Density Network Structure (GPR w/ WhiteKernel Sampling)

### Layers

- **9** Hidden **relu** layers
- **1** Hidden **tanh** layer for smoothness
- Mixture Density layer (output)

### Neurons
**100** neurons/layer

### Number of mixes (Gaussians)
**3** mixes

# Citing
The main publication (and documentation) to cite is:

- Vasilis Tsioulos and Vaia Prassa, "Mixture density network in evaluating incomplete fission mass yields", Volume 60, article number 182, (2024) The European Physical Journal A, DOI: [10.1140/epja/s10050-024-01409-0](https://doi.org/10.1140/epja/s10050-024-01409-0)

Demonstration of a workflow to

1. calibrate a population-average model using cross-sectional data
2. derive a individual-specific model from a population-average model

## Workflow
1. calibration of population-average model
2. reduce parameter space based on sensitivity analysis
3. define prior parameter distributions based on a MCMC sampling applied on the population-average model
4. update population parameters in a Bayesian approach -> individual parameter set 

### Calibration of the population-average model (cross-sectional data)

![Alt text](https://github.com/SoFiwork/CrossSectional2individual/blob/main/Workflow.svg)

### Updating to an individual-specific model (simulated data)

![Alt text](https://github.com/SoFiwork/CrossSectional2individual/blob/main/BayesianWorkflow.svg)

## Model 

dyanmic model (system of ordinary differential equations) describing the hormone dynamics of three reproductive hormones during puberty in girls

![Alt text](https://github.com/SoFiwork/CrossSectional2individual/blob/main/PubertyFlow.pdf)

## Installation
The model is written in Python 3. 

To run the demo, clone the repository:

```
git clone https://github.com/SoFiwork/CrossSectionsl2Individual
```

Create an virtual environment from \textit{BayesianUpdating2023.yaml} to use the same package versions that has been used when creating the demo. 
When using anaconda run 

```
conda env create -f BayesianUpdating2023.yaml
```

in the correct directory 

## Simulation demos 

summary of files used to generate the results presented in the corresponding publication 

### Pipeline_PopulationModel.ipynb

implentation of the work steps illustrated under ``Calibration of the population-average model''

Steps: 
1. Maximum likelihood (ML) estimation of the population parameters using averaged cross-sectional data 
2. Calculation of Likelihood Profiles around the ML estimate
3. Uncertainty quntification: MCMC sampling from the likelihood function of the population average model 
4. Sobol sensitivity analysis

Figure 4, 5, 7, A1b from Fischer-Holzhausen et al. 2023 can be reproduced with this file. 
Note that results will be comparable, but details might differ because the methods are sampling based (a seed has not been set). 

OptimizationResult.pkg are the MLE results used for the figure in Fischer-Holzhausen et al. 2023

### Pipeline_IndividualModel_SimulatedIndividual.ipynb 

implentation of the work steps illustrated under ``Updating to an individual-specific model''

The estimation of prior distributions is discussed in Fischer-Holzhausen et al. 2023. 
The generation of a synthetic dataset is also explained in Fischer-Holzhausen et al. 2023. 

Figure 9 from Fischer-Holzhausen et al. 2023 can be reproduced with this file. 
Note that results will be comparable, but details might differ because the methods are sampling based (a seed has not been set). 

## License
This model is licensed under the MIT License.

## Citation


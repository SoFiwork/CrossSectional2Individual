# Demonstration of Bayesian updating workflow: translate a population-average model into a individual-specific model 

## Model 

dyanmic model (system of ordinary differential equations) describing the hormone dynamics of three reproductive hormones during puberty in girls

![Alt text](https://github.com/SoFiwork/CrossSectional2individual/blob/main/PubertyFlow.pdf)

## Workflow
1. calibration of population-average model
2. reduce parameter space based on sensitivity analysis
3. define prior parameter distributions based on a MCMC sampling applied on the population-average model
4. update population parameters in a Bayesian approach -> individual parameter set 

### Calibration of the population-average model (cross-sectional data)

![Alt text](https://github.com/SoFiwork/CrossSectional2individual/blob/main/Workflow.svg)

### Updating to an individual-specific model (simulated data)

![Alt text](https://github.com/SoFiwork/CrossSectional2individual/blob/main/BayesianWorkflow.svg)

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

### Pipeline_IndividualModel_SimulatedIndividual.ipynb 

implentation of the work steps illustrated under ``Updating to an individual-specific model''

## License
This model is licensed under the MIT License.

## Citation


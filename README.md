# Demonstration of Bayesian updating workflow: translate a population-average model into a individual-specific model 

## model: dyanmic model (system of ordinary differential equations) describing the hormone dynamics of three reproductive hormones during puberty in girls

![Alt text](https://github.com/SoFiwork/GynCycle_newVersion/blob/main/Flowchart.jpg)

## workflow presented in the corresponding article 
1. calibration of population-average model
2. reduce parameter space based on sensitivity analysis
3. define prior parameter distributions based on a MCMC sampling applied on the population-average model
4. update population parameters in a Bayesian approach -> individual parameter set 

## Description 
Mathematical model of the female menstrual cycle that couples the dynamics between follicles and hormones.

![Alt text](https://github.com/SoFiwork/GynCycle_newVersion/blob/main/Flowchart.jpg)

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

## Demo 

### Pipeline_IndividualModel_SimulatedIndividual.ipynb 

### Pipeline_PopulationModel.ipynb


## License
This model is licensed under the MIT License.

## Citation


# Plan Overview

## Simulation Shape:
An hourglass like figure will be used with 2 bottlenecks introduced in the simulation
- Bottleneck 1: Patient Admission
- Bottleneck 2: The Discharge Process

## Behavior
The patients will navigate these environments where ER and OPD patients will be used as agent templates
- The parameters will be drawn from a distribution set for their templates to add variability to behavior
 
### Mortality
- This behavior will be a simple variable assigned with a fixed value with variability applied via a random choice amongst a normal distribution of the said variable
  
- With admission (the state of the patient being assigned admitted to the hospital simulation) their mortality will decrease based off a set value with varied distribution applied normally.
  
- The mortality rate will change dependant on variables of:
  - number of patients under a physician agents service (inverse relationship)
  - these changes occur only in the circumstance of there being bed availability which is set as an absolute threshold of the model for admission

### Discharge
Occurs when mortality value is below a chosen threshold


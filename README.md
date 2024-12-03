# Plan Overview

## Simulation Shape:
An hourglass like figure will be used with 2 bottlenecks introduced in the simulation
- Bottleneck 1: Patient Admission funnels into bottleneck 2 as it empties.
- Bottleneck 2: The Hospital Ward

## Behavior
The patients will navigate these environments where patients will be used as agent templates
- The parameters will be drawn from a normal distribution set for their templates to add variability to behavior

### Patient Parameters
- mortality
- waiting_time
- discharge_probability
- category
 
### Mortality
- This behavior will be a simple variable assigned with a fixed value with variability applied via a random choice amongst a normal distribution of the said variable
  
- With admission (the state of the patient being assigned admitted to the hospital simulation) their mortality will decrease based off a set value with varied distribution applied normally.
  
- The mortality rate will change dependant on variables of:
  - number of patients under a physician agents service (inverse relationship)
  - The waiting time outside of admission (positive relationship)

### Discharge
- Patients will have a default rate of 0.5 upon entering the hospital, as they stay in the hospital this rate will go up by 0.1 (+/-) a chosen normal distribution to add variability
- This discharge rate could change in relation to the patient category
 - patients with a rare condition for example could have a slower discharge progression due to unfamiliarity


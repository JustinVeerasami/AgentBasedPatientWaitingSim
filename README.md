# Agent Based Patient Waiting Simulation
Agent-Based Modeling of Patient Waiting for Hospitalization and Different Prioritization Strategies

## Background and introduction
- Patients evaluated in the emergency department (ER) or during outpatient
visits (OPD) may need admission for further treatment. The waiting time 
for a hospital bed varies based on patient acuity, bed availability, and 
hospital capacity.
- Hospital admission notifications can be prioritized differently, such as 
prioritizing emergency patients, those waiting longer, or reserving beds 
for educational purposes. Different strategies affect patient mortality rate,
waiting times and resident physician learning outcomes.

## Objective
- This study aims to simulate the effects of different admission notification 
strategies on patient mortality rates, waiting times, and physician learning
outcomes with agent-based modeling.

Goal: Find the best admission notification strategy to reduce patient mortality rates, waiting times, and improve physician learning outcomes.

## Methodology
Each patient is an agent.
- There are 2 different types of agents: from the ER or from the OPD.
- The properties of each agent include mortality rate, recovery rate, waiting time, educational value, and probability of being discharged tomorrow.
- Each property is generated with different initial value distributions based on the type of agent, and these properties may change over time and with the environment.
The hospital team capacity is the environment.
- There are 3 medical teams in the inpatient ward.
- The properties of each medical team include capacity for patients, efficiency for discharge, and learning outcomes, which change with the agents they encounter.
Simulation: choose different prioritizations of patient admissions based on their type, waiting time, disease acuity, and educational value.



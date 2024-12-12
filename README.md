# Agent Based Patient Waiting Simulation
Agent-Based Modeling of Patient Waiting for Hospitalization and Different Prioritization Strategies

<div align="center">
  <img src="https://github.com/user-attachments/assets/cf13303a-99e3-4d5e-bab7-c686df352b03" alt="Patient_Waiting_gif-ezgif com-crop (1)">
</div>


## Background and introduction
Patients evaluated in the emergency department (ER) or during outpatient
visits (OPD) may need admission for further treatments. The waiting time 
for a hospital bed varies based on:

- patient acuity
- bed availability
- hospital capacity

Hospital admission notifications can be prioritized differently, such as:
- prioritizing emergency patients
- patient waiting time
- reserving beds for educational purposes

Different strategies affect patient mortality rate,
waiting times and resident physician learning outcomes.

## Objectives
This study aims to simulate the effects of different admission notification 
strategies with agent-based modeling on:
- patient mortality rates
- waiting times
- physician learning outcomes

### Goal
Find the best admission notification strategy to reduce patient mortality rates, waiting times, and improve physician learning outcomes.

# Methodology
### Each patient is an agent.
- There are 2 different types of agents:
  - from the ER
  - from the OPD.
- The properties of each agent include
  - mortality rate
  - recovery rate
  - waiting time
  - educational value
  - probability of being discharged tomorrow.
- Each property is generated with different initial value distributions based on the type of agent, and these properties may change over time and with the environment.
  
### The hospital team capacity is the environment
- There are 3 medical teams in the inpatient ward.
- The properties of each medical team include
  - capacity for patients
  - efficiency for discharge
  - learning outcomes, which change with the agents they encounter
  
## Simulation
Choose different prioritizations of patient admissions based on their 
- type
- waiting time
- disease acuity
- educational value

## Installation
Steps to run the simulation:

1. Clone the github repository:
    ```bash
    git clone -b main https://github.com/JustinVeerasami/AgentBasedPatientWaitingSim.git
    ```

2. Navigate to the project directory:
    ```bash
    cd AgentBasedPatientWaitingSim
    ```

3. Install the required dependencies using pip:
    ```bash
    pip install -r requirements.txt
    ```
## Run The Simulation
```bash
python main.py
```


## Reference Papers
1.	Emergency departments for reducing patient waiting times. PLoS One. Jul 2 2009;4(7):e6127. doi:10.1371/journal.pone.0006127
2.	Kim J-K. Enhancing Patient Flow in Emergency Departments: A Machine Learning and Simulation-Based Resource Scheduling Approach. Applied Sciences. 2024;14(10)doi:10.3390/app14104264



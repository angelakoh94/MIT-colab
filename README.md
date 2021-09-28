# MIT-colab
We will be looking at patients who have arterial and venous blood gases measured very close to each other. This will provide an estimate of how much oxygen is extracted by the tissues from the arterial blood and how much carbon dioxide is dumped into the venous blood. These are proxies for cellular metabolism during critical illness.
We will be using MIMIC-IV dataset for this project.

Variables to obtain: Blood gas measurements: pO2, pCO2, pH, O2 saturation %, lactate + HR, BP, FiO2, mechanically ventilated from LABEVENTS dataset (d_labitems dataset gives the list of measurements), age, SOFA score, comorbidity 
Timestamp: storetime not charttime

Couplets of central venous and arterial blood gases (O2 and CO2) within 1 hour, excluding if there are: Intubation between collection
Don’t stratify by time period, obtain ALL available data 

Central venous saturation (on blood gas) - ALL available data

Lactate levels within 4 hours pre and post collection (both arterial & venous), 2 types (serum lactate vs. bg measurement → collect both types), all lactate measurements within 8hr window (pre AND post)

Vasopressors and inotropes including doses DURING bg measurement from prescriptions dataset -epinephrine, norepinephrine, dobutamine, dopamine, phenylephrine, milrinone and vasopressin

Central line only
PICC line, internal jugular, subclavian acceptable
not Femoral central line

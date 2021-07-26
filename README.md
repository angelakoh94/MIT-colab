# MIT-colab
We will be looking at patients who have arterial and venous blood gases measured very close to each other. This will provide an estimate of how much oxygen is extracted by the tissues from the arterial blood and how much carbon dioxide is dumped into the venous blood. These are proxies for cellular metabolism during critical illness.
We will be using MIMIC-IV dataset for this project.

Variables to obtain: LABEVENTS dataset (d_labitems dataset gives the list of measurements)

Couplets of central **venous** and **arterial** blood gases within 1 hour, excluding if there are: Intubation between collection (pO2:50821, pCO2:50818)

Central venous saturation (on blood gas) (Oxygen Saturation:50817)

Lactate levels within 4 hours pre and post collection (Lactate:50813, 52442)

Vasopressors and inotropes including doses  - need to find the name of medications 

Central line presence, and location

    PICC line, internal jugular, subclavian acceptable

    Femoral central line?
    
    

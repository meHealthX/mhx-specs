# MEP 2: Data - Digital Health
This MEP explains and sets the scope of digital health data for our
purpose.

The basic idea is that it covers the data related to the diverse set of apps
and platforms generating and storing data related to the patients' health.
For instance:

- Clue/Flo: keeps track of the users' menstruation cycle and related symptoms
- Fitbit: generates data related to the phisical activity of the user
- MedAngel: tracks fridge temperature of stocked insulin for the patients

These all produce and/store data directly related to the health and treatment
of the patients and the users.

We can assume the following main attributes for them:

- owner: the patient about whom the data is
- creator: the app/platform having produced the data
- holder: the party holding and storing the data
- metadata: metadata explaining what the data is. For instance:
  - pain
  - menstruation
  - migraine
  - medicine sensors
- data: the data itself

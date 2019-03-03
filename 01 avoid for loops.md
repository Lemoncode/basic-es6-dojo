# Avoiding for loops

Blog: https://www.basefactor.com/es6-for-loops-forget-it

# The data collection set

```javacript
const patients = [
  {
    id: 1,
    name: 'John',
    lastname: 'Doe',
    sex: 'Male',
    temperature: 36.8,
    heartRate: 80,
    specialty: 'general medicine',
    age: 44,
  },
  {
    id: 2,
    name: 'Jane',
    lastname: 'Doe',
    sex: 'Female',
    temperature: 36.8,
    heartRate: 70,
    specialty: 'general medicine',
    age: 43,
  },
  {
    id: 3,
    name: 'Junior',
    lastname: 'Doe',
    sex: 'Male',
    temperature: 36.8,
    heartRate: 90,
    specialty: 'pediatrics',
    age: 8,
  },
  {
    id: 4,
    name: 'Mary',
    lastname: 'Wien',
    sex: 'Female',
    temperature: 36.8,
    heartRate: 120,
    specialty: 'general medicine',
    age: 20,
  },
  {
    id: 5,
    name: 'Scarlett',
    lastname: 'Somez',
    sex: 'Female',
    temperature: 36.8,
    heartRate: 110,
    specialty: 'general medicine',
    age: 30,
  },
  {
    id: 6,
    name: 'Brian',
    lastname: 'Kid',
    sex: 'Male',
    temperature: 39.8,
    heartRate: 80,
    specialty: 'pediatrics',
    age: 11,
  },
];
```

# Excercise 1:

a) We've got the list of patients we want to extract a list of
patients that are assigned to _pediatrics_ specialty.

b) We want to narrow down that list to patients assigned to
_pediatrics_ and _age_ below 10 years old.

# Excercise 2:

We want to activate the urgency protocol if any of the patients
heart rate is above 100 or temperature is greater than 39 Celsius.

# Excercise 3:

The Pediatrician could not attend today the patients: We want to reassign patients assigned to _pediatrics_ specialty to
_general medicine_

# Excercise 4

We want to know if we can send the Pediatrician home (no patients today),
check if any patient is assigned to _pediatrics_

# Excercise 5:

We want to calculate the total of patients that are assigned
to general medicine and the number of patients that are assigned
to pediatrics.

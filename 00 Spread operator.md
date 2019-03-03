# About spread operator

Official MDN documentation: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Spread_syntax

Blog post: https://davidwalsh.name/spread-operator

# Excercise 1: Update single property first level

Let's say we have a default patient template, and we want
to create a helper mehtod to create a new patient informing
the name and lastname fields (this helper method should
take as starting point the object created in defaultPatient
and it should create a new object and update the field
without mutating the original defaultPatient).

```javascript
const defaultPatient = {
  id: -1,
  name: "",
  lastname: "",
  sex: "Male",
  temperature: 36.8,
  heartRate: 100,
  specialty: "general medicine"
};

const createNewPatient = (name, lastname) => {
  // Your code here
};

const newPatient = createNewPatient("John", "Doe");

console.log(newPatient);
console.log(defaultPatient);
```

# Excercise 2: Update single property nested object

Let's start from this new patient template:

```javascript
const defaultPatient = {
  id: -1,
  name: "",
  lastname: "",
  sex: "Male",
  sensors: {
    temperature: 36.8,
    heartRate: 100
  },
  specialty: "general medicine"
};
```

Now we want to create a new object and update the _temperature_ field,
we will take as starting point _defaultPatient_ and we will create
a new object without mutating the original.

```javascript
const defaultPatient = {
  id: -1,
  name: "",
  lastname: "",
  sex: "Male",
  sensors: {
    temperature: 36.8,
    heartRate: 100
  },
  specialty: "general medicine"
};

const createNewPatient = temperature => {
  // Your code here, update temperature field
};

const newPatient = createNewPatient(38);

console.log(newPatient);
console.log(defaultPatient);
```

# Excercise 3: Indicate property name + value

Now we want to inform the id of the field to update plus the value,
then it should create a new object with the value updated.

```javascript
const defaultPatient = {
  id: -1,
  name: "",
  lastname: "",
  sex: "Male",
  temperature: 36.8,
  heartRate: 100,
  specialty: "general medicine"
};

const updatePatientInmutable = (fieldId, fieldValue, patient) => {
  // Your code here
};

const newPatient = updatePatientInmutable("lastname", "Doe");

console.log(newPatient);
console.log(defaultPatient);
```

# Excercise 4: Add new element to array

We have a list of patients (Array) and we want to add a new patient
to that list without mutating the list.

```javascript
const patients = [
  {
    id: 1,
    name: 'John',
    lastname: 'Doe',
    sex: 'Male'
    temperature: 36.8,
    heartRate: 100,
    specialty: 'general medicine',
  },
  {
    id: 2,
    name: 'Jane',
    lastname: 'Doe',
    sex: 'Female'
    temperature: 36.8,
    heartRate: 100,
    specialty: 'general medicine',
  },
];

const newPatient =   {
    id: 2,
    name: 'Junior',
    lastname: 'Doe',
    sex: 'Male'
    temperature: 36.8,
    heartRate: 100,
    specialty: 'pediatrics',
  };

const newPatientCollection = addPatient(newPatient, patients) => {
  // your code here
}

console.log(patients);
console.log(newPatientCollection);
```

# Excercise 5: Concat arrays

We want to concat two list of patients without mutating any of the
original ones, how can we do that using spread operator?

```javascript
const patientsFloor2 = [
  {
    id: 1,
    name: 'John',
    lastname: 'Doe',
    sex: 'Male'
    temperature: 36.8,
    heartRate: 100,
    specialty: 'general medicine',
  },
  {
    id: 2,
    name: 'Jane',
    lastname: 'Doe',
    sex: 'Female'
    temperature: 36.8,
    heartRate: 100,
    specialty: 'general medicine',
  },
];


const patientsFloor3 = [
  {
    id: 1,
    name: 'Mary',
    lastname: 'Wien',
    sex: 'Female'
    temperature: 36.8,
    heartRate: 100,
    specialty: 'general medicine',
  },
  {
    id: 2,
    name: 'Scarlett',
    lastname: 'Somez',
    sex: 'Female'
    temperature: 36.8,
    heartRate: 100,
    specialty: 'general medicine',
  },
];

const contactPatients(patientCollectionA, patientCollectionB) => {
  // your code here
}

const totalCollection = concatPatients(patientsFloor2, patientsFloor3);

console.log(patientsFloor2);
console.log(patientsFloor3);
console.log(totalCollection);
```

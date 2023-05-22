## Class 4 Extra Practice Key

#### Exercise 1

```js
let studentData = {
  studentName: 'Javi',
  cityOfOrigin: 'Madrid',
  age: 34,
};

for (key in studentData) {
  console.log(studentData[key]);
}
```

#### Exercise 2

```js
let newData = [
  ['major', 'philosophy'],
  ['classesRegistered', 5],
];

let newDataObject = Object.fromEntries(newData);
console.log(newDataObject);

Object.assign(studentData, newDataObject);
console.log(studentData);
```

## Class 3 Extra Practice Key

#### Object Practice - Part 1

```js
let studentData = {
  studentName: 'Javi',
  cityOfOrigin: 'Madrid',
  age: 34,
  major: 'Literature',
  registeredClasses: 4,
  greeting() {
    console.log(
      `Hello my name is ${this.studentName}; I'm ${this.age} years old; and I'm from ${this.cityOfOrigin}.`
    );
  },
};
```

#### Object Practice - Part 2

```js
studentData.studentName = 'Carla';
studentData.age = 32;
delete studentData.major;
console.log(studentData);
```

#### Object Practice - Part 3

```js
studentData.declareMajor = function (major) {
  console.log(
    `I'm studying ${major}, and I'm registered for ${this.registeredClasses} classes this semester.`
  );
};

console.log(studentData);
studentData.declareMajor('Architecture');
```

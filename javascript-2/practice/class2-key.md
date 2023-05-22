## Class 2 Extra Practice Key

#### Exercise 1

```js
let oneNameSingers = ['Beyonce', 'Cher', 'Bjork', 'Sia'];

let uppercaseNames = oneNameSingers.map((singer) => {
  return singer.toUpperCase();
});
```

#### Exercise 2

```js
let largeNumbers = [300, 24, 9350, -2, 147, 59];

let smallNumbers = largeNumbers.filter((number) => {
  return number < 100;
});
```

#### Exercise 3

```js
let singularNouns = ['pen', 'book', 'house', 'bike'];

singularNouns.forEach((noun) => {
  console.log(noun + 's');
});
```

#### Exercise 4

```js
let checkNumbers = [4, 10, 56, 34];

let checkNumbersResult = checkNumbers.every((num) => {
  return num % 2 === 0;
});
```

#### Exercise 5

```js
let catStrings = ['avocado', 'advocate', 'catty', 'catacomb'];

let findCatString = catStrings.find((word) => word.includes('cat'));
```

#### Exercise 6

```js
let findCatString2 = catStrings.findIndex((word) => word.includes('cat'));
```

#### Exercise 7

```js
let planets = ['Mercury', 'Venus', 'Jupiter'];

let duplicatePlanets = [];

planets.forEach((planet) => duplicatePlanets.push(planet));

console.log(duplicatePlanets);
```

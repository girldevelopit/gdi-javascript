## Class 1 Extra Practice Key

#### Part 1

Code should display:

```js
"This week's lineup at Madison Square Garden:
 - beyonce
 - drake
 - billie eilish
 - coldplay"
```

#### Part 2 & 3 - Refactoring with ES6

```js
const theatre = 'Madison Square Garden';

let artists = ['beyonce', 'drake', 'billie eilish', 'coldplay'];

const billboard = () => {
  let announcement = `This week's lineup at ${theatre}:`;

  for (let artist of artists) {
    announcement += `
- ${artist.toUpperCase()}`;
  }

  return announcement;
};

let displayBillboard = billboard();

console.log(displayBillboard);
```

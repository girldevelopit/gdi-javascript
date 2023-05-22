## Class 1 Extra Practice

#### Part 1

Copy and paste the code below into a code editor or console window:

```js
var theatre = 'Madison Square Garden';

var artists = ['beyonce', 'drake', 'billie eilish', 'coldplay'];

function billboard() {
  var announcement = "This week's lineup at " + theatre + ':';

  for (var i = 0; i < artists.length; i++) {
    announcement = announcement + '\n - ' + artists[i];
  }

  return announcement;
}

var displayBillboard = billboard();

console.log(displayBillboard);
```

#### Part 2 - Refactor

Update the code in Part 1 using the new ES6 syntax we've learned in class!

- Replace all the `var` declarations with `const` or `let`
- Rewrite the function as an arrow function
- Replace all string concatenation with string interpolation
- Replace the `for` loop with a `for of` loop
- Run the code to make sure the same output is displayed

#### Part 3 - Bonus Challenges

- In the `for of` loop, use the compound assignment operator to update the 'announcement' variable

  - Hint: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators

- Output each artist's name in uppercase
  - Hint: Go to MDN and lookup a string method for this

---

See how far you can get before going to the solution key--ideally no more than 30-45 minutes overall.

_Solution Key: class1-key.md_
_(Update this page's url with the solution key's file name)_

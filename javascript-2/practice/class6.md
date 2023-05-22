## Class 6 Github Practice

#### Part 1

Create an `index.html` file and paste the following code in between the body tags:

```html
<h2>Display Your Github Profile Image and URL!</h2>
<div class="container">
  <div class="img-box"></div>
  <div class="text-box">
    <h3 class="name-data"></h3>
    <p>
      <a
        href=""
        target="_blank"
        class="url-data"
        >Github URL</a
      >
    </p>
  </div>
</div>
<script src="promise.js"></script>
```

#### Part 2

Create a `style.css` file and paste the following code into the file, then make sure to link the stylesheet to the `index.html` file

OR

Add the code in between `<style></style>` tags in the `index.html` file:

```css
body {
  font-family: 'Josefin Sans', sans-serif;
  color: rgb(82, 82, 82);
}

h2 {
  text-align: center;
}

.container {
  max-width: 200px;
  width: 100%;
  border: 4px solid rgb(246 67 166);
  margin: 0 auto;
  border-radius: 0.5rem;
  overflow: hidden;
}

img {
  display: block;
  max-width: 100%;
}

.text-box {
  padding: 2rem 0.5rem;
  text-align: center;
}

h3,
p {
  margin: 0;
}

h3 {
  font-size: 1.5rem;
  text-transform: uppercase;
  margin-bottom: 0.75rem;
}

a,
a:active,
a:visited {
  color: rgb(82, 82, 82);
}

a:hover {
  color: rgb(246 67 166);
}
```

#### Part 3

Create a `promise.js` file and paste the following code into the script file:

```js
let githubImage = document.createElement('img');

let imageBox = document.querySelector('.img-box');

imageBox.appendChild(githubImage);

let githubName = document.querySelector('.name-data');

let githubURL = document.querySelector('.url-data');
```

#### Part 4

The setup for the exercise is now complete. Open the `index.html` file in a browser. You should have a simple display that looks similar to this:

https://girldevelopit.github.io/gdi-javascript/javascript-2/images/github-api-starter.png

#### Part 5

Copy and paste the JavaScript code below into the `promise.js` file after the `githubURL` variable declaration

```js
let githubAPI = 'https://api.github.com/search/users?q=tinuola'

let myGithubProfile = fetch( ??? )
.then( (???) => ??? )
.then( (???) => {
  console.log(???) /* Tip: Log data to console */

  // githubImage.src = /* use the avatar_url property */

  // githubName.innerHTML = /* use the login property */

  // githubURL.href = /* use the html_url property */
})
.catch( (???) => console.log(???) )
```

#### Part 6

Using the API demo/examples covered in class, update the code from Part 5 by completing the following steps:

a. Update the query string at the end of the `githubAPI` url from 'tinuola' to your github username (or any Github username)

b. Pass the githubAPI variable from step A into the fetch method (Remove the ???)

c. Fill out the two `.then()` methods and the `.catch()` method (Remove the ???)

d. Log the returned data--this will help you determine how to extract the value(s) you need

e. Once you've identified the `key:value` pairs you need, assign them to their appropriate DOM objects/elements (githubImage.src, githubName.innerHTML, githubURL.href)

f. Open or refresh `index.html` in your browser. You should have an updated display that looks similar to this--with your selected Github profile name, url and image:

https://girldevelopit.github.io/gdi-javascript/javascript-2/images/github-api-completed.png

#### Part 7 - Optional

a. Update the CSS styling if you prefer

b. Use JavaScript, instead of CSS, to uppercase your username

c. Use string interpolation or concatenation to add a unique error message to the `err` variable in the `.catch()` method; then create a minor error (ex: mistype a variable or a fake github username) so you can log/see the error message

d. If you have DOM manipulation knowledge, then retrieve other data from the API call and add them to the page!

---

See how far you can get before going to the solution key--ideally no more than 30-45 minutes overall.

_Solution Key: class6-key.md_
_(Update this page's url with the solution key's file name)_

## Class 6 Github Practice Key

#### Part 6 & 7

```js
let githubAPI = 'https://api.github.com/search/users?q=tinuola';

let myGithubProfile = fetch(githubAPI)
  .then((res) => res.json())
  .then((data) => {
    console.log(data);

    let myData = data.items[0];

    githubImage.src = myData.avatar_url;

    githubName.innerHTML = myData.login;
    // githubName.innerHTML = myData.login.toUpperCase()

    githubURL.href = myData.html_url;
  })
  .catch((err) => console.log(`Darn, something went wrong! 😭 ${err}`));
```

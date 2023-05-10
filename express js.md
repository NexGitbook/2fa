# Express JS

### Install packages

```
npm i express nodemon
```

### Create app/index.js

```js
const express = require('express');

const app = express();

app.get('/', (req, res) => {
  res.send('Hello Express app!')
});

app.listen(3000, () => {
  console.log('server started');
});
```

### Start Server

```
nodemon app/index.js
```
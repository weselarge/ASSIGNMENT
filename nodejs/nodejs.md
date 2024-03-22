# QUESTION 3: NODEJS
## Requirement:
* Dockerfile
* app.js
* express package

* Dockerfile: Create a file with the touch cmd and populate with the code below:

FROM node:16.14.0-alpine
WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 3000

CMD [ "node", "app.js" ][image](./nodeJs1.png)

* app.js: This is the application file. Create the app file and populate with this code:

const express = require('express');

const app = express();

const PORT = process.env.PORT || 3000;

app.get('/', (req, res) => {
  res.send('Hello Adewale, Welcome Docker! with NodeJS');
});

app.listen(PORT, () => {
  console.log(`Server running on port ${PORT}`);
});[image](./appNoJs.png)

*   express package: Install the express package with the nodejs package manager: 

        npm install express
*Note: The above installation will generate node_modules, package.json and package-lock.json in your main directory.

Build the Dockerfile, then run the image

[Output on your browser](./nodeJsWEBSITE.png))






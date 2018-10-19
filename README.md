
# mongoose-serverless

mongoose-serverless is for mongoose connections in serverless (function paradigm).
```js
const myMongo = require('mongoose-serverless');

...
const urlConnection = '<urlConnectonMongoose>'

async function doSomethingWithDB() {
    try {
        await myMongo.connectToDatabase(urlConnection);
        // mongoose queries
    } catch (e) {
        throw new Error(e);
    }
}
...
```

# Install

```console
$ npm install mongoose-serverless
```

# Contribute

If there is a new model you would like to support, or want to add a direct conversion between two existing models, please send us a pull request.

# License
Copyright &copy; 2018, Abraham Silva. Licensed under the [ISC License](LICENSE).
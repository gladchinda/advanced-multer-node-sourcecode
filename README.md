# advanced-multer-node-sourcecode

**You can checkout the complete tutorial on Scotch: [Advanced Photo Upload in Node](https://scotch.io/tutorials/advanced-photo-upload-in-node).**

Source code for tutorial on advanced photo upload in Node using Multer and Jimp. In order to run the demo on your local machine and experiment with the source code, do the following:

- Clone the repository into a new directory on your machine

- Run the following command from the new directory to install the dependencies:

```sh
npm install --save express lodash body-parser morgan cookie-parser debug ejs serve-favicon multer jimp dotenv concat-stream streamifier mkdirp
```

- Create a `.env` file in the root of the new directory with the following content:

```ini

# Avatar Upload Variables

AVATAR_FIELD=avatar
AVATAR_BASE_URL=/uploads/avatars
AVATAR_STORAGE=public/uploads/avatars

```

- The app will run on port **3000** by default. If you would prefer another port, you can specify it in the `bin/www` file. Look for the following line in the file and replace `'3000'` with your desired port.

```js
var port = normalizePort(process.env.PORT || '3000');
```

- Finally, start the demo app by running the following command:

```sh
npm start
```

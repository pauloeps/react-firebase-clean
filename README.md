# React Firebase Clean

This project is intended to be an implementation of a Clean Architecture on a structure using React as the main frontend library, and firebase as the backend. The Clean Architecture is implemented specifically on the firebase functions folder, in the `./functions` directory.

## How To Run

To run the project, you will need first to run the command `npm install` at the root folder to install all the dependencies. Next, create a `.env.local` file with the following variables (the values will be filled later):

* REACT_APP_APIKEY
* REACT_APP_AUTHDOMAIN
* REACT_APP_PROJECTID
* REACT_APP_STORAGEBUCKET
* REACT_APP_MESSAGINGSENDERID
* REACT_APP_APPID
* REACT_APP_MEASUREMENTID

Now you need to create a firebase project [here](https://console.firebase.google.com). After creating the project, add a web app. In the project configuration, you will be able to find in the SDK configuration section, a JavaScript code with a `firebaseConfig` object. This is the same code found on `services/firebase.js`, and the keys on the `firebaseConfig` object are the same keys that you created earlier on the `.env.local` file, now you only need to fill them correctly.
# GeoBook front-end README

To view a demo of the app, please visit: https://vimeo.com/823682896?share=copy

## About

This is a final group project I worked on while on the Northcoders software development bootcamp.

GeoBook is a geocaching app that allows users to hide and collect books anywhere accross the world.

On the interactive map screen, the app tracks your location (if the user allows permissions) and displays books markers at locations where books can be found. Once a user has found a book, they can swap the book with one they've alredy read. Users can also add new books at new locations.

The user area allows users to view a list of books they've previously found.

## Back-end

The Github repository for the back-end can be found here: https://github.com/beckybp/be-nc-geobook

## Minimum version of Node required

The minimum version of Node required to run locally is v19.3.0

## How to set up this project locally

To set up this project locally please follow the steps below:

1. Fork this repository.

2. Clone this repository to your local machine and cd into it:
```
$ git clone <repo-url>
$ cd fe-nc-geobook
```
3. You will need to create a file in the root directory called 'firebaseConfig.js' and include the following code, adding your own Firebase config details.
```
import { initializeApp } from "firebase/app";
import { getAuth } from "firebase/auth";

const firebaseConfig = {
  apiKey: "addYourApiKeyHere", //replace with your details
  authDomain: "addYourAuthDomainHere", //replace with your details
  projectId: "addYourProjectIdHere", //replace with your details
  storageBucket: "addYourStorageBucketHere", //replace with your details
  messagingSenderId: "addYourMessagingSenderIdHere", //replace with your details
  appId: "addYourAppIdHere" //replace with your details
};

const app = initializeApp(firebaseConfig);
export const auth = getAuth(app);
export default app
```

4. Install all dev dependencies:
```
npm install
```

5. To view the app run:
```
npx expo
```

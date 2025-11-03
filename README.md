<h1>Linking a database to a react app</h1>

STEP1:
Setting up fire base

first navigate to ["https://firebase.google.com/"](firebase.com)

Sign in or sign up to access the firebase dashboard.

Set up a new project this will be the project that we will be using to store the data base.

Set up a firestore database. From here you can structure the database how you like. 

STEP2:
You will be given an api key and all the config code in a snippet. This is then added to a page in your react website. 

<code>
const firebaseConfig = {
  apiKey: “API_KEY”,
  authDomain: “DOMAIN”,
  projectId: “PROJECT_”ID,
  storageBucket: “STORAGE_BUCKET”,
  messagingSenderId: “SENDER_ID”,
  appId: “APP_ID”
};
</code>

Import the firebase dependencies in the header of your react page.

<code>
import { initializeApp } from 'firebase/app';
import { getFirestore, collection, getDocs, doc, setDoc ,addDoc} from 'firebase/firestore/lite';
import { getStorage, ref, uploadBytes } from "firebase/storage";
</code>

<hr>
TASK1:
Sett up a react app that adds the user’s name and email address to a firebase database.

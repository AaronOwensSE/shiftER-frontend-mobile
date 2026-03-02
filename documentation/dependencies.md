# Dependencies

- React - Custom UI components with props, style, and state
- React Native - React for mobile devices
- Expo SecureStore - Secure local storage of credentials

## Setup

### From Repo

If App.js, app.json, index.js, package.json, and package-lock.json are present (as they should be), frontend setup is straightforward.

From the frontend root:

```
npm install
```

Then, use .env.example as a guide to set environment variables in .env.

### From Scratch

Generally speaking, it is not viable to set up an Expo project from scratch as a configuration step for an already existing project. Creating a new Expo project overwrites existing files, including App.js and index.js, which should not be overwritten.

If, for some reason, app.json, package.json, and package-lock.json need to be recreated, they can be copied over from a new Expo project created in a *separate directory* to avoid overwriting.

From a *safe directory* not containing project files:

```
npx create-expo-app frontend --template blank
npx expo install expo-secure-store
```

Then, app.json, package.json, and package-lock.json can be copied to the project directory, and normal setup can be performed.

---

[Back to README](../README.md)

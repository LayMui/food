# This is a qa app for design system testing

To get started create the project using expo-cli

1. npx expo-cli init qaappdesignsystem
2. npm install -g expo-cli
3. Install react-navigation to allow user to navigate around
   npm install react-navigation
4. Install other Dependencies
   expo install react-native-gesture-handler react-native-reanimated react-native-screens react-native-safe-area-context @react-native-community/masked-view
5. Install React Navigation Stack
   npm install react-navigation-stack @react-native-community/masked-view

6. Start the app and clear cache with expo r -c

React Navigation v4 Docs:
https://reactnavigation.org/docs/4.x/getting-started

## Convert expo to react native project

expo eject
yarn ios
yarn android

### To build ipa file on xcode

1. Select the Targets: qaappdesignsystem
2. Go to Product -> Archive
3. Click on Distribute App
4. Click Development
5. App Thinning: All compatible device variants
6. Automatically manage signing
7. Export

### Access bit.dev

Login to bit.dev

```
https://bit.dev/yaradigital/ahua-design-system
```

### Install Ahua component

Example: AhuaButton

```
 yarn add @yaradigital/ahua-design-system.ui.button
```

will add the dependencies to the package.json as shown:

```"dependencies": {
    "@yaradigital/ahua-design-system.ui.button": "^0.0.13",

```

Add fonts

https://www.bigbinary.com/learn-react-native/adding-custom-fonts

for this

```
<Button
        type='Primary'
        title='Loading Button'
        loading={true}
        iconPlacement='LEFTICON'
      />
```

Add the config file react-native.config.js

reference:
https://www.bigbinary.com/learn-react-native/adding-custom-fonts

### Install react-native-svg for ios only

```
yarn add react-native-svg
cd ios
pod install
```

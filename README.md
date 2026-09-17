# Movie Mobile App

A cross-platform movie app built with Expo, React Native, TypeScript, Expo Router, and NativeWind.

## Requirements

- Node.js 22.13 or later
- npm
- Android Studio for Android development, or Xcode for iOS development

This project uses Expo SDK 57 and React Native 0.86.

## Getting started

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm start
```

Then choose a target from the Expo CLI, or use one of the platform commands:

```bash
npm run android
npm run ios
npm run web
```

Use `npx expo start --clear` if Metro's cache needs to be reset.

## Available scripts

| Command           | Description                       |
| ----------------- | --------------------------------- |
| `npm start`       | Start the Expo development server |
| `npm run android` | Start the app for Android         |
| `npm run ios`     | Start the app for iOS             |
| `npm run web`     | Start the web version             |
| `npm run lint`    | Run Expo linting                  |

## Project structure

```text
src/
  app/
    _layout.tsx       # Root Expo Router layout
    index.tsx         # Home screen
    global.css        # NativeWind entry stylesheet
metro.config.js       # Expo and NativeWind Metro configuration
tailwind.config.js    # NativeWind class scanning and theme configuration
```

Routes are defined in `src/app` using [Expo Router](https://docs.expo.dev/router/introduction). Styling uses [NativeWind](https://www.nativewind.dev/) utility classes.

## Verification

Check Expo package compatibility:

```bash
npx expo install --check
```

Create an Android production bundle:

```bash
npx expo export --platform android
```

## Resources

- [Expo SDK 57 documentation](https://docs.expo.dev/versions/v57.0.0/)
- [Expo Router documentation](https://docs.expo.dev/router/introduction)
- [NativeWind documentation](https://www.nativewind.dev/)

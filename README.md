# Expo Managed Workflow Compatibility Issues

This repository demonstrates a common issue encountered when developing Expo managed workflow applications: compatibility problems with native modules or functionalities that aren't supported by the Expo Go app or EAS Build.  The example showcases how attempting to access functionalities that require direct device access causes runtime errors.

## Setup

1. Clone the repository.
2. `npm install`
3. Run the project using `expo start`.

## Bug Reproduction

The `bug.js` file attempts to use a hypothetical native module that's not Expo-compatible.  This will result in an error when running the app in Expo Go or building it with EAS Build.

## Solution

The `bugSolution.js` file demonstrates the correct approach: utilizing Expo APIs to access the device's functionality.  In this case, the appropriate Expo module (if available) provides a cross-platform and safe way to interact with the underlying functionality.
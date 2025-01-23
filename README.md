# React Native AsyncStorage Inconsistent Null Return Bug

This repository demonstrates a bug where `AsyncStorage.getItem` in React Native inconsistently returns `null`, even when data exists.  The issue is intermittent and challenging to debug using standard null checks.

## Bug Reproduction

1. Clone this repository.
2. Run `npm install`.
3. Run the app on an emulator or device.
4. Observe the inconsistent behavior of `AsyncStorage.getItem`. Sometimes it retrieves data, other times it returns `null` even though the data is present.

## Solution

The provided solution utilizes promises and error handling to reliably retrieve data from AsyncStorage, providing a workaround for the intermittent null return issue. 
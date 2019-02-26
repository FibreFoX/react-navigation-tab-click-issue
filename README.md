# Reproducable example project

Following commands were used to create this project:
* `react-native init reactnavigationtabissue --version react-native@next --template typescript`
* `yarn add react-navigation`
* `yarn add react-native-gesture-handler`
* `react-native link react-native-gesture-handler`


## What this project is about

When using the tab-feature via [`createMaterialTopTabNavigator()`](https://reactnavigation.org/docs/en/material-top-tab-navigator.html), clicking the second tab, it switches to the content, as expected. But when clicking the first tab again, the content **does not switch back**, but can be reached via swipe. I think this is a bug, maybe due to ReactNative 0.59 RC2?!

Tested on Android Emulator and real-device.

This issue was reported here: https://github.com/react-navigation/react-navigation/issues/5629
# my-app
"In case you want to run my attachments, make sure you follow these steps to use react-navigation v4 in them:

1) Run npm install and then expo upgrade

2) Install all extra navigators that are required for this specific code snapshot:

npm install --save react-navigation-stack

npm install --save react-navigation-tabs

npm install --save react-navigation-drawer

(of course you can combine that all into one npm install command if you need all of them)

3) Make sure you're using version 4 of react-navigation

npm install --save react-navigation@latest

4) Install all required dependencies

expo install react-native-gesture-handler react-native-reanimated react-native-screens react-native-safe-area-context @react-native-community/masked-view

5) Update all "navigator" imports

import { createStackNavigator, createAppContainer } from 'react-navigation';

would become

import { createAppContainer } from 'react-navigation';
import { createStackNavigator } from 'react-navigation-stack';
for example. Do that for all navigators (e.g. tabs, drawer) you might be using in the specific snapshot.

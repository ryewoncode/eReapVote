<template>
  <view class="container">
    <header title="TooPyo" />
    <!-- <app-navigator></app-navigator> -->
    <view class="view-Contents">
      <home />
    </view>
    <bottom-nav />
  </view>
</template>

<script>
// import {
//   createAppContainer,
//   createStackNavigator,
// } from "vue-native-router"

import Header from "./src/view/Layout/Header"
import BottomNav from "./src/view/Layout/BottomNav/BottomNavigator"
import Home from "./src/view/Layout/BottomNav/Home"
// import Notice from "./src/view/Layout/Notice"

// const StackNavigator = createStackNavigator(
//   {
//     Home: Home,
//     Details: Notice,
//   },
//   {
//     initialRouteName: 'Home',
//   }
// );

// const AppNavigator = createAppContainer(StackNavigator);

export default {
  components : {
    Header,
    Home,
    // AppNavigator, 
    BottomNav
  }
}
</script>

<style>
.container {
  background-color: white;
  flex: 1;
}
.view-Contents {
  background-color: #F5F5F8;
  flex: 1;
  align-items: stretch;
  padding: 5px;
}
</style>

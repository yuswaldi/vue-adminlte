<template>
  <!-- <div id="app"> -->
    <div class="wrapper">
      <!-- <app-header v-if="isAuth" /> -->
      <app-header />

      <!-- Left side column. contains the logo and sidebar -->
      <sidebar />

      <div class="content-wrapper">
        <router-view></router-view>
      </div>
      <!-- <app-footer v-if="isAuth" /> -->
    </div>
  <!-- </div> -->
</template>

<script>
import Sidebar from './layout/Sidebar';
import Header from './layout/Header';

export default {
  name: 'MainLayout',
  components: {
    // DashFooter,
    'app-header' : Header,
    Sidebar
  }
};
</script>
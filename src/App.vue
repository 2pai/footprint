<template>
    <v-app class="grey lighten-5">
      <v-content>
      <v-container class="pt-12">
          <h1 class="display-2 text-justify text-capitalize font-weight-medium">
                  2Pai footprint 👣
          </h1>
          <router-view></router-view>
      </v-container>
      </v-content>
    </v-app>
</template>

<script>
export default {
  name: 'App'
  
  // components:{
  //   Blog
  // }
};
</script>
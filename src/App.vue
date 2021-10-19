<template>
  <v-app>
    <v-app-bar
        fixed
        app
        flat
        color="insta"
    >
      <div class="toolbar-container">
        <v-toolbar-title v-text="'Портфолио'"/>
        <v-spacer/>
        <v-btn
            icon
            @click.stop="rightDrawer = !rightDrawer"
        >
          <v-icon>send</v-icon>
        </v-btn>
      </div>
    </v-app-bar>
    <v-container>
      <v-main>
        <Profile />
        <v-divider class="my-4"> </v-divider>
        <div class="d-flex align-center justify-center mb-4">
          <v-icon>
            grid_on
          </v-icon>
          <span>Проекты:</span>
        </div>
        <Grid />
      </v-main>
    </v-container>
  </v-app>
</template>

<script>

import Profile from './components/Profile'
import Grid from './components/Grid'

export default {
  name: 'App',
  data: () => ({
  }),
  components: {
    Profile, Grid
  }
};
</script>

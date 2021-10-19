<template>
  <v-dialog
      transition="dialog-bottom-transition"
      v-model="dialog"
      max-width="600"
  >
    <template v-slot:activator="{ on, attrs }">
      <v-card flat
              @mouseover="changeColor = !changeColor"
              @mouseout="changeColor = !changeColor"
              class="card"
              v-on="on"
      >
        <v-img :src="require(`@/assets/${project.img}`)" cover/>
      </v-card>
    </template>


    <v-card class="modal">
      <video :src="require(`@/assets/sites/${project.video}`)" width="400" height="300" controls="controls" class="modal__video"></video>
      <v-card-title>
        {{ project.title }}
      </v-card-title>
      <v-card-text>
        {{ project.subtitle }}
      </v-card-text>
    </v-card>
  </v-dialog>
</template>

<script>
export default {
  props: {
    project: {
      type: Object,
      default: () => {
      }
    }
  },
  data() {
    return {
      changeColor: false,
      dialog: false
    }
  },
  methods: {},
  computed: {}
}
</script>

<style>

</style>

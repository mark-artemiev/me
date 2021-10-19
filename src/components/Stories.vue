<template>
  <div class="d-flex my-10">
    <div v-for="(item, index) in blocks"
         :key="index"
         :item="item"
         class="dir mx-8"
    >
      <v-img
             class="rounded-circle"
             :src="setPhoto"
             max-height="80"
             max-width="80"
      />
      <p class="text-center">
        Кто я?
      </p>
    </div>

  </div>
</template>

<script>
export default {
  data () {
    return {
      blocks: [
        '1', '2', '3'
      ]
    }
  },
  computed: {
    setPhoto () {
      return require("@/assets/unnamed.jpg")
    }
  }
}
</script>

<style scoped>

</style>

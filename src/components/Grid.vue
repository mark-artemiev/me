<template>
  <v-row justify="center" align="center">
    <v-col cols="12" md="6" lg="4" v-for="(item, index) in projects" :key="index">
      <Project :project="item"/>
    </v-col>
  </v-row>
</template>

<script>
import Project from './Project'

export default {
  components: { Project },
  data() {
    return {
      projects: [
        {
          id: 1,
          video: '1.mp4',
          img: '1.png',
          title: 'Интернет-магазин очков и аксессуаров',
          subtitle: 'Вёрстка интернет-магазина, реализация логики работы с корзиной заказов, оформление заказа, оплата'
        },
        {
          id: 2,
          video: '2.mp4',
          img: '2.png',
          title: 'Портал управляющей компании',
          subtitle: 'Вёрстка главного портала, реализация логики для передачи показаний по счётчикам. Реализация личного кабинета.'
        },
        {
          id: 3,
          video: '3.mp4',
          img: '3.png',
          title: 'Сайт визитка для хостинговой компании',
          subtitle: 'Вёрстка слайдера-лендинга.'
        },
        {
          id: 4,
          video: '4.mp4',
          img: '4.png',
          title: 'Сайт для стоматологической клиники',
          subtitle: 'Вёрстка.'
        },
        {
          id: 5,
          video: '5.mp4',
          img: '5.png',
          title: 'Сайт агенства интернет-маркетинга',
          subtitle: 'Вёрстка. Реализация сложных svg анимаций.'
        },
        {
          id: 6,
          video: '6.mp4',
          img: '6.png',
          title: 'Интернет-магазин по продаже мотособак',
          subtitle: 'Вёрстка. Реализация логики на клиентской стороне.'
        },
      ]
    }
  },
  methods: {},
  computed: {}
}
</script>

<style scoped>

</style>

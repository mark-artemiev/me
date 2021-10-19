<template>
      <v-card flat class="d-flex justify-space-around">
        <v-row justify="center" align="center" class="mt-3">
          <v-col  cols="12" md="4">
        <v-img class="rounded-circle" :src="require('@/assets/unnamed.jpg')" max-height="250" max-width="250" />
          </v-col>
            <v-col cols="12" md="8">
        <div class="profile__stats">
          <div class="d-flex align-center">
            <h2> Марк Артемьев</h2>
<!--            <v-btn color="primary" text>Написать</v-btn>-->
          </div>
          <ul class="stats__menu">
            <li>
              <strong>38</strong> проектов
            </li>
            <li>
              <strong>3</strong> года опыта
<!--              <small>коммерческого опыта разработки</small>-->
            </li>
            <li>
              <strong>24</strong> отзыва
<!--              <small>от довольных заказчиков</small>-->
            </li>
          </ul>
          <div class="profile__description">
            Я веб-разработчик с особенным вниманием к деталям и 3х-летним опытом разработки. Пишу чистый, поддерживаемый код.
            Имею большой опыт верстки шаблонных и уникальных сайтов. Работаю с анимацией и SVG. Работал как в веб-студиях с различными по тематике проектами,
            так и в продуктовых компаниях, создавал высоконагруженные и сложные приложения. Без проблем могу сверстать страницу под ваши запросы.
          </div>
        </div>
            </v-col>
        </v-row>
      </v-card>
</template>

<script>
export default {
  data () {
    return {
      projects: [
        '1', '2', '3', '4', '5', '6'
      ]
    }
  },
  computed: {
  }
}
</script>

<style scoped>

</style>

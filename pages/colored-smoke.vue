<template>
  <section class="landing-wrap">
    <main class="main">
      <div class="container">
        <div class="main-left">
          <h1 class="section-title big gradient">Цветной дым</h1>
          <h3 class="main-subtitle">Сделай фотосессию <br>невероятно <br>завораживающей</h3>
          <div class="main-buttons">
            <div class="main-btn__wrap">
              <nuxt-link to="/catalog/?category=2" class="btn">Перейти в магазин</nuxt-link>
              <p class="landing__label">от 330 рублей за штуку</p>
            </div>
          </div>
        </div>
      </div>
    </main>
    <section class="about">
      <div class="container">
        <h2 class="section-title big gradient">Что такое цветной дым?</h2>
        <p class="subtitle">Густые клубы дыма, вызывающие восторг</p>
        <p class="about-text">Цветной дым — это абсолютно безопасный вид пиротехники. При активации дымовой шашки выходит окрашенный густой дым, клубы которого очень эффектно смотрятся в реальности, на фото и видео.</p>
        <div class="about-images">
          <div class="about-image"><img src="../assets/img/landings/smoke/about-1.png" alt=""></div>
          <div class="about-image"><img src="../assets/img/landings/smoke/about-2.png" alt=""></div>
          <div class="about-image"><img src="../assets/img/landings/smoke/about-3.png" alt=""></div>
        </div>
        <p class="subtitle blue">Где и когда пригодится дым</p>
        <div class="about-using">
          <div class="about-using__item">
            <div class="about-using__img"><img src="../assets/img/icons/photo-camera.svg" alt=""></div>
            <p class="about-using__text">Фото съемка</p>
          </div>
          <div class="about-using__item">
            <div class="about-using__img"><img src="../assets/img/icons/movie-clapper-open.svg" alt=""></div>
            <p class="about-using__text">Видео продакшн</p>
          </div>
          <div class="about-using__item">
            <div class="about-using__img"><img src="../assets/img/icons/speech.svg" alt=""></div>
            <p class="about-using__text">Митинги или акции</p>
          </div>
          <div class="about-using__item">
            <div class="about-using__img"><img src="../assets/img/icons/people-watching-a-movie.svg" alt=""></div>
            <p class="about-using__text">Шоу и концерты</p>
          </div>
          <div class="about-using__item">
            <div class="about-using__img"><img src="../assets/img/icons/puzzle.svg" alt=""></div>
            <p class="about-using__text">Квесты и игры</p>
          </div>
          <div class="about-using__item">
            <div class="about-using__img"><img src="../assets/img/icons/man-in-a-party.svg" alt=""></div>
            <p class="about-using__text">Массовые мероприятия</p>
          </div>
        </div>
        <nuxt-link to="/catalog/?category=2" class="btn centred">Перейти в магазин</nuxt-link>
      </div>
    </section>
    <section class="about-second">
      <parallax-container class="about-second__right-bg">
        <parallax-element :factor=".4">
          <img src="../assets/img/landings/smoke/about-second__right.png" alt="" class="about-second__right-bg--img">
        </parallax-element>
      </parallax-container>
      <div class="container flex jc-sb">
        <button @click="openVideo($store.state.shop.settings[6].value)" class="about-second__left video-btn">
          <span class="video-btn__body gradient"></span>
          <span class="video-btn--label-1">Смотреть видео</span>
        </button>
        <div class="about-second__right">
          <h2 class="section-title big gradient">Как дымит шашка?</h2>
          <p class="subtitle">Посмотрите видео цветного дыма в действии</p>
          <p class="about-second__text">Цветной дым — безопасная пиротехника, которая не красит одежду, кожу, волосы. Среднее время дымления шашки от 40 до 60 секунд.</p>
          <small class="about-second__small">*Для полной безопасности необходимо соблюдать инструкцию и рекомендации, написанные на этикетке шашки</small>
        </div>
      </div>
    </section>
    <section class="features">
      <div class="container">
        <h2 class="section-title big gradient">Преимущества цветного дыма</h2>
        <p class="subtitle">Почему стоит купить цветной дым в магазине HOLIDAY PAINT?</p>
        <div class="features-body flex jc-sb">
          <div class="features-left">
            <div class="features-img"><img src="../assets/img/landings/smoke/colors.png" alt=""></div>
            <p class="features-label">Более 9 цветов</p>
          </div>
          <ul class="features-list">
            <li class="features-list__item">
              <div class="features-list__img"><img src="../assets/img/icons/wool.svg" alt=""></div>
              <span class="features-list__text">Статичные и ручные</span>
            </li>
            <li class="features-list__item">
              <div class="features-list__img"><img src="../assets/img/icons/list-with-bullets.svg" alt=""></div>
              <span class="features-list__text">5 производителей шашек</span>
            </li>
            <li class="features-list__item">
              <div class="features-list__img"><img src="../assets/img/icons/timing.svg" alt=""></div>
              <span class="features-list__text">Дымление до 120 секунд</span>
            </li>
            <li class="features-list__item">
              <div class="features-list__img"><img src="../assets/img/icons/cloud.svg" alt=""></div>
              <span class="features-list__text">Насыщенный и густой</span>
            </li>
          </ul>
        </div>
          <nuxt-link to="/catalog/?category=2" class="btn centred">Перейти в магазин</nuxt-link>
      </div>
    </section>
    <section class="feedback">
      <div class="container">
        <h2 class="section-title big gradient">Фото с цветным дымом</h2>
        <p class="subtitle">Мы запечатлели самые яркие жизненные моменты</p>
        <feedbacks/>
        <nuxt-link to="/catalog/?category=2" class="btn centred">Перейти в магазин</nuxt-link>
      </div>
    </section>
    <section class="faq">
      <div class="container">
        <h2 class="section-title big gradient">FAQ</h2>
        <p class="subtitle">Часто задаваемые вопросы про цветной дым</p>
        <div class="faq-body">
          <el-collapse v-model="activeCollapses">
            <el-collapse-item title="Сколько дымит дымовая шашка?" name="1">
              <div>Шашки дымят от 30 до 120 секунд, в зависимости от модели, но в основном у нас представлены шашки с дымлением 60 секунд.</div>
            </el-collapse-item>
            <el-collapse-item title="Сколько видов цвета дыма?" name="2">
              <div>У нас представлены более 9 видов цвета дыма.</div>
            </el-collapse-item>
            <el-collapse-item title="Пачкает дым одежду?" name="3">
              <div>Цветной дым не пачкает одежду если соблюдать инструкцию по применению. не направляйте факел дыма близко к человеку и не держите его в направлении одежды более 2 секунд.</div>
            </el-collapse-item>
            <el-collapse-item title="Можно держать в руке?" name="4">
              <div>Производитель не рекомендует держать шашку в руке, но её можно взять за нижнюю часть где она не будет нагреваться и держать на вытянутой руке под углом. Мощные шашки нужно использовать только на земле согласно инструкции по пременению.</div>
            </el-collapse-item>
          </el-collapse>
        </div>
      </div>
    </section>
    <popular-goods/>
    <el-dialog
      :visible.sync="videoDialog"
      custom-class="video-dialog"
      @closed="videoUrl = ''"
    >
      <iframe
        class="dialog-video"
        width="100%"
        height="100%"
        :src="videoUrl">
      </iframe>
    </el-dialog>
  </section>
</template>

<script>

  import Parallax from 'parallax-js'
  import Feedbacks from "../components/Feedbacks";
  import PopularGoods from "../components/PopularGoods";
  export default {
    components: {
      PopularGoods,
      Feedbacks
    },
    head: {
      title: `Holiday Paint | Главная`
    },
    data: () => ({
      videoDialog: false,
      videoUrl: null,
      activeCollapses: ['1'],
    }),
    methods: {
      openVideo(link) {
        this.videoUrl = 'https://www.youtube.com/embed/' + link.split('/').pop()
        this.videoDialog = true
      }
    },
    mounted() {
      console.log(this.$store.state.shop.settings)
    },
  }
</script>

<style lang="scss" scoped>
  @import "../assets/sass/variables";
  /*LANDING*/
  .btn.centred {
    width: fit-content;
    margin-left: auto;
    margin-right: auto;
  }
  .landing {
    &-list {
      margin-bottom: 1.5em;
      &__item {
        display: flex;
        align-items: center;
        font-size: 1.5em;
        &:not(:last-child) {
          margin-bottom: 1em;
        }
      }
      &__text {
        @media (max-width: 600px) {
          font-size: .85em;
        }
      }
      &__icon {
        margin-right: 1em;
        min-width: 2em;
        width: 2em;
        height: 2em;
        border-radius: 50%;
        background-color: #fff;
        display: flex;
        align-items: center;
        justify-content: center;
        box-shadow: 0 4px 11px rgba(168, 168, 168, 0.21);
        img {
          height: .9em;
        }
      }
    }
    &-label {
      font-size: 1.5em;
      margin-bottom: 1.5em;
      @media (max-width: 600px) {
        text-align: center;
      }
    }
  }
  @media (max-width: 600px) {
    h2.section-title.big {
      font-size: 2.5em;
    }
    p.subtitle {
      font-size: 1.5em;
    }
  }
  /*HOME END*/

  /* MAIN */
  h1.section-title {
    margin-top: .25em;
    font-size: 4.5em;
    text-align: left;
    margin-bottom: 0.15em;
    @media (max-width: 600px) {
      text-align: center;
      font-size: 4em;
    }
  }
  p.subtitle.blue {
    text-transform: uppercase;
    text-align: center;
  }
  .main {
    position: relative;
    padding-bottom: 8em;
    @media (max-width: 1440px) {
      padding-bottom: 10em;
    }
    @media (max-width: 768px) {
      padding-bottom: 6em;
    }
    &:after {
      content: '';
      width: 100%;
      height: calc(100% + 14em);
      right: 0;
      top: -14em;
      position: absolute;
      background-image: url('../assets/img/landings/smoke/main-bg.png');
      background-position: right top;
      background-repeat: no-repeat;
      background-size: auto 100%;
      z-index: -1;
      @media (max-width: 1440px) {
        right: -10%;
      }
      @media (max-width: 1024px) {
        top: -6em;
        background-size: auto 85%;
        right: -15%;
      }
      @media (max-width: 600px) {
        content: none;
      }
    }
    .container {
      display: flex;
    }
    &-subtitle {
      text-align: left;
      font-size: 3em;
      color: $blue;
      font-weight: 600;
      margin-bottom: 1em;
      @media (max-width: 600px) {
        text-align: center;
        font-size: 2.5em;

      }
    }
    &-btn__wrap {
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    &-buttons {
      display: flex;
      align-items: center;
      font-size: 1.4em;
      @media (max-width: 600px) {
        flex-direction: column;
      }
      .landing__label {
        height: 1.5em;
        margin-top: 1em;

      }
      .btn {
        padding-left: 3.5em;
        padding-right: 3.5em;
      }
      .video-btn {
        z-index: 1;
        margin-left: 2em;
        margin-bottom: 2.5em;
        @media (max-width: 600px) {
          margin-left: 0;
          margin-bottom: 4.5em;
          order: -1;
        }
        &--label-1 {
          z-index: -2;
        }
      }
    }
    &-left {
      width: 65%;
      @media (max-width: 1024px) {
        width: 70%;
      }
      @media (max-width: 900px) {
        width: 80%;
      }
      @media (max-width: 600px) {
        font-size: .8em;
        width: 100%;
        text-align: center;
      }
    }
  }

  /*MAIN END*/

  /* ABOUT */

  .about {
    position: relative;
    &-bg {
      width: 15%;
      top: 0;
      position: absolute;
      left: 0%;
      @media (max-width: 768px) {
        display: none;
      }
    }
    &-images {
      display: flex;
      justify-content: space-around;
      margin-bottom: 2em;
      flex-wrap: wrap;
    }
    &-image {
      text-align: center;
      width: 30%;
      @media (max-width: 600px) {
        width: 90%;
      }
      img {
        width: 100%;
      }
    }
    .subtitle {
      margin-bottom: 1.5em;
    }
    &-text {
      font-size:  1.5em;
      text-align: center;
      width: 40em;
      max-width: 100%;
      margin-left: auto;
      margin-right: auto;
      margin-bottom: 2em;
    }
    &-facts {
      display: flex;
      align-items: flex-end;
      justify-content: space-between;
      margin-bottom: 4em;
      flex-wrap: wrap;
      @media (max-width: 768px) {
        justify-content: space-around;
      }
    }
    &-fact {
      @media (max-width: 768px) {
        width: 49%;
        &:not(:last-child) {
          margin-bottom: 2em;
        }
      }
      @media (max-width: 600px) {
        width: 100%;
      }
      &__img {
        height: 6em;
        text-align: center;
        margin-bottom: 1em;
        img {
          height: 100%;
        }
      }
      &__text {
        text-align: center;
        font-size: 1.5em;
      }
      &:last-child {
        .about-fact__img {
          height: 11em;
          img {
            height: 120%;
          }
        }
      }
    }
    &-using {
      display: flex;
      justify-content: space-between;
      margin-bottom: 3em;
      flex-wrap: wrap;
      @media (max-width: 768px) {
        justify-content: space-around;
        margin-bottom: 1em;
      }
      &__item {
        width: 16%;
        text-align: center;
        @media (max-width: 768px) {
          width: 32%;
          margin-bottom: 2em;
        }
      }
      &__img {
        height: 5em;
        width: 5em;
        margin-left: auto;
        margin-right: auto;
        margin-bottom: 1em;
        padding: 1.25em 0;
        text-align: center;
        background-image: url('../assets/img/landings/about-item-bg.png');
        background-position: center;
        background-repeat: no-repeat;
        background-size: contain;
        img {
          height: 2.5em;
        }
      }
    }

    &-second {
      padding: 15em 0;
      background-image: url('../assets/img/landings/smoke/about-second__bg.png');
      background-position: left center;
      background-repeat: no-repeat;
      background-size: auto 100%;
      position: relative;
      &__right-bg {
        position: absolute;
        right: 0;
        top: 40%;
        transform: translateY(-50%);
        width: 18%;
        z-index: -1;
      }
      @media (max-width: 1600px) {
        background-size: 45% auto;
        &__right-bg {
          width: 15%;
        }
      }
      @media (max-width: 768px) {
        background-image: none;
        padding: 8em 0 4em;
        &__right-bg {
          display: none;
        }
        .container {
          flex-direction: column;
        }
      }
      .video-btn {
        margin-right: auto;
        margin-left: 0;
        @media (min-width: 769px) {
          &--label-1 {
            display: none;
          }
        }
        @media (max-width: 768px) {
          order: 1;
          margin-top: 2em;
          margin-left: auto;
          &--label-1 {
            left: 50%;
            top: 100%;
            text-align: center;
            transform: translateX(-50%)
          }
        }
      }
      &__right {
        width: 57%;
        @media (max-width: 768px) {
          width: 100%;
          text-align: center;
        }
      }
      .section-title {
        text-align: left;
        width: 10em;
        max-width: 100%;
        margin-bottom: .25em;
        @media (max-width: 768px) {
          text-align: center;
          margin-left: auto;
          margin-right: auto;
        }
      }
      .subtitle {
        text-align: left;
        margin-bottom: 2em;
        @media (max-width: 768px) {
          text-align: center;
        }
      }
      &__text {
        font-size: 1.5em;
        width: 27em;
        max-width: 100%;
        margin-bottom: 1.5em;
        @media (max-width: 768px) {
          margin-left: auto;
          margin-right: auto;
        }
      }
    }
  }

  /* ABOUT END */

  /* FEATURES */

  .features {
    padding: 5em 0;
    .section-title {
      margin-bottom: .5em;
    }
    &-left {
      width: 50%;
      text-align: center;
      @media (max-width: 767px) {
        width: 100%;
        margin-bottom: 2em;
      }
    }
    &-body {
      flex-wrap: wrap;
      margin-bottom: 2em;
    }
    &-img {
      width: 25em;
      max-width: 100%;
      margin-left: auto;
      margin-right: auto;
      margin-bottom: 2em;
      img {
        width: 100%;
      }
    }
    &-label {
      font-size: 1.5em;
    }
    &-list {
      width: 50%;
      @media (max-width: 767px) {
        width: 100%;
      }
      &__item {
        display: flex;
        align-items: center;
        font-size: 1.5em;
        height: 3.5em;
        position: relative;
        @media (max-width: 768px) {
          font-size: 1.25em;
        }
      }
      &__img {
        width: 2em;
        height: 2em;
        min-width: 2em;
        display: flex;
        align-items: center;
        justify-content: center;
        background-color: #fff;
        border-radius: 50%;
        box-shadow: 0 4px 11px rgba(168, 168, 168, 0.21);
        margin-right: 1em;
        img {
          height: .8em;
        }
      }

    }

  }

  /* FEATURES END */

  /* FEEDBACKS */

  .feedback {
    &-slider {
      padding-bottom: 4em;
    }
  }


  /* FEEDBACKS END*/

  /* FAQ */

  .faq {
    padding: 5em 0;
  }

  /* FAQ END*/

</style>

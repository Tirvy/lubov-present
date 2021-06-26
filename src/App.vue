<template>
  <div id="app">
    <swiper>
      <swiper-slide v-for="(item, index) in slides" :key="index">
        <component :is="item"></component>
      </swiper-slide>
    </swiper>
  </div>
</template>

<script>
import { Swiper, SwiperSlide, directive } from 'vue-awesome-swiper'

// import style (>= Swiper 6.x)
import 'swiper/swiper-bundle.css'

import Slide1 from './components/Slide1Space';
import Slide2 from './components/Slide2Travel';
import Slide3 from './components/Slide3Bridge';
import Slide4 from './components/Slide4BridgeCloud';
import Slide5 from './components/Slide5BridgeFormer';
import Slide6 from './components/Slide6BridgeFormerWork';
import Slide7 from './components/Slide7BridgeFormerDissapear';
import Slide8 from './components/Slide8BridgeDrop';
import Slide9 from './components/Slide9GivePresents';

export default {
  name: 'App',
  components: {Swiper, SwiperSlide},
  data() {
    return {slides: [Slide1, Slide2, Slide3, Slide4, Slide5, Slide6, Slide7, Slide8, Slide9]}
  },
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.slide-container {
  position: relative;
  width: 1200px;
  height: 675px;
}

.lubov-captain,
.zays,
.former {
  filter: drop-shadow(2px 2px 0 white) 
          drop-shadow(-2px -2px 0 white);
}

@keyframes shake {
  10%, 90% {
    transform: translate3d(-1px, 0, 0);
  }
  
  20%, 80% {
    transform: translate3d(2px, 0, 0);
  }

  30%, 50%, 70% {
    transform: translate3d(-4px, 0, 0);
  }

  40%, 60% {
    transform: translate3d(4px, 0, 0);
  }
}

@keyframes sway {
  0%, 100% {
    transform: translate3d(-14px, 0, 0);
  }
  25% {
    transform: translate3d(0, 14px, 0);
  }
  50% {
    transform: translate3d(14px, 0, 0);
  }
}

@keyframes spin { 100% { -webkit-transform: rotate(360deg); transform:rotate(360deg); } }
</style>

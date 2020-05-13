<template>
  <div id="app">
    <Carousel
      v-model="value1"
      loop
      :height="600"
    >
        <CarouselItem>
            <div class="demo-carousel">
              云。。。。
            </div>
        </CarouselItem>
        <CarouselItem>
            <div class="demo-carousel">smile</div>
        </CarouselItem>
        <CarouselItem>
            <div class="demo-carousel">
              <img src="./assets/qb.jpg" alt="">
            </div>
        </CarouselItem>
    </Carousel>
    <img src="./assets/me.jpeg" alt="" class="qb">
  </div>
</template>

<script>
import Vue from 'vue';
import Component from 'vue-class-component';
import {
  Carousel,
  CarouselItem,
} from 'iview';
import './common/css/global.css';
export default @Component({
  name: 'App',
  components: {
    Carousel,
    CarouselItem,
  }
})
class App extends Vue {
  value1 = 0;
}
</script>

<style lang="less">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  .demo-carousel{
    width: 100%;
    height: 100%;
    text-align: center;
    font-size: 16px;
    background: #506b9e;
    color: #fff;
    img{
      width: 100%;
      height: 100%;
    }
  }
  .qb{
    margin-top: 20px;
  }
}
</style>

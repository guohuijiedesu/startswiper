<template>
  <div class="custom">
    <swiper :options="swiperOption" ref="mySwiper">
      <swiper-slide>
        <img src="./../assets/1.jpg"/><img src="./../assets/2.jpg"/><img src="./../assets/3.jpg"/><img src="./../assets/4.jpg"/><img src="./../assets/5.jpg"/>
        <img src="./../assets/6.jpg"/><img src="./../assets/7.jpg"/><img src="./../assets/8.jpg"/><img src="./../assets/9.jpg"/><img src="./../assets/10.jpg"/>
        <img src="./../assets/11.jpg"/><img src="./../assets/12.jpg"/><img src="./../assets/13.jpg"/><img src="./../assets/14.jpg"/><img src="./../assets/15.jpg"/>
      </swiper-slide>
      <swiper-slide>
        <img src="./../assets/16.jpg"/><img src="./../assets/17.jpg"/><img src="./../assets/18.jpg"/><img src="./../assets/19.jpg"/><img src="./../assets/20.jpg"/>
        <img src="./../assets/21.jpg"/><img src="./../assets/22.jpg"/><img src="./../assets/23.jpg"/><img src="./../assets/24.jpg"/><img src="./../assets/25.jpg"/>
        <img src="./../assets/26.jpg"/><img src="./../assets/27.jpg"/><img src="./../assets/28.jpg"/><img src="./../assets/29.jpg"/><img src="./../assets/30.jpg"/>
      </swiper-slide>
      <swiper-slide>
        <img src="./../assets/31.jpg"/><img src="./../assets/32.jpg"/><img src="./../assets/33.jpg"/><img src="./../assets/34.jpg"/><img src="./../assets/35.jpg"/>
        <img src="./../assets/36.jpg"/><img src="./../assets/37.jpg"/><img src="./../assets/38.jpg"/><img src="./../assets/39.jpg"/><img src="./../assets/40.jpg"/>
        <img src="./../assets/41.jpg"/><img src="./../assets/42.jpg"/><img src="./../assets/43.jpg"/><img src="./../assets/44.jpg"/><img src="./../assets/45.jpg"/>
      </swiper-slide>
      <swiper-slide>
        <img src="./../assets/46.jpg"/><img src="./../assets/47.jpg"/><img src="./../assets/48.jpg"/><img src="./../assets/49.jpg"/><img src="./../assets/40.jpg"/>
        <img src="./../assets/51.jpg"/><img src="./../assets/52.jpg"/><img src="./../assets/53.jpg"/><img src="./../assets/54.jpg"/><img src="./../assets/55.jpg"/>
        <img src="./../assets/56.jpg"/><img src="./../assets/57.jpg"/><img src="./../assets/58.jpg"/><img src="./../assets/59.jpg"/><img src="./../assets/60.png"/>
      </swiper-slide>
      <swiper-slide>
        <img src="./../assets/61.jpg"/><img src="./../assets/62.jpg"/><img src="./../assets/63.jpg"/><img src="./../assets/64.jpg"/><img src="./../assets/65.jpg"/>
        <img src="./../assets/66.jpg"/><img src="./../assets/67.jpg"/><img src="./../assets/68.jpg"/><img src="./../assets/69.jpg"/><img src="./../assets/70.jpg"/>
        <img src="./../assets/71.jpg"/><img src="./../assets/72.jpg"/><img src="./../assets/73.png"/><img src="./../assets/74.png"/><img src="./../assets/75.png"/>
      </swiper-slide>
      <swiper-slide>
        <img src="./../assets/76.jpg"/><img src="./../assets/77.jpg"/><img src="./../assets/78.jpg"/><img src="./../assets/79.jpg"/><img src="./../assets/80.jpg"/>
        <img src="./../assets/81.png"/><img src="./../assets/82.jpg"/><img src="./../assets/83.jpg"/><img src="./../assets/84.jpg"/><img src="./../assets/85.png"/>
        <img src="./../assets/86.png"/><img src="./../assets/87.jpg"/><img src="./../assets/88.jpg"/><img src="./../assets/89.jpg"/><img src="./../assets/90.png"/>
      </swiper-slide>
      <swiper-slide>
        <img src="./../assets/91.jpg"/><img src="./../assets/92.jpg"/><img src="./../assets/93.jpg"/><img src="./../assets/94.jpg"/><img src="./../assets/95.jpg"/>
        <img src="./../assets/96.png"/><img src="./../assets/97.jpg"/><img src="./../assets/98.jpg"/><img src="./../assets/99.jpg"/><img src="./../assets/100.jpg"/>
        <img src="./../assets/101.jpg"/><img src="./../assets/102.jpg"/><img src="./../assets/103.png"/><img src="./../assets/104.jpg"/><img src="./../assets/105.jpg"/>
      </swiper-slide>
      <swiper-slide>
        <img src="./../assets/106.jpg"/><img src="./../assets/107.jpg"/><img src="./../assets/108.jpg"/><img src="./../assets/109.jpg"/><img src="./../assets/120.jpg"/>
        <img src="./../assets/111.jpg"/><img src="./../assets/112.jpg"/><img src="./../assets/113.jpg"/><img src="./../assets/114.jpg"/><img src="./../assets/115.png"/>
        <img src="./../assets/116.jpg"/><img src="./../assets/117.jpg"/><img src="./../assets/118.jpg"/><img src="./../assets/119.jpg"/><img src="./../assets/120.jpg"/>
      </swiper-slide>
      <swiper-slide>
        <img src="./../assets/121.jpg"/><img src="./../assets/122.jpg"/><img src="./../assets/123.jpg"/><img src="./../assets/124.jpg"/><img src="./../assets/5.jpg"/>
        <img src="./../assets/126.jpg"/><img src="./../assets/127.png"/><img src="./../assets/128.jpg"/><img src="./../assets/129.jpg"/><img src="./../assets/120.jpg"/>
        <img src="./../assets/131.jpg"/><img src="./../assets/132.jpg"/><img src="./../assets/133.jpg"/><img src="./../assets/134.jpg"/><img src="./../assets/135.jpg"/>
      </swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
// 引入插件
import { swiper, swiperSlide } from "vue-awesome-swiper";
import "swiper/dist/css/swiper.css";

export default {
  components: {
    swiper,
    swiperSlide
  },
  data() {
    return {
      swiperOption: {
        loop: true,
        autoplay: {
          delay: 3000,
          stopOnLastSlide: false,
          disableOnInteraction: false
        },
        pagination: {
          el: ".swiper-pagination",
          bulletClass : 'my-bullet',
          bulletActiveClass: 'my-bullet-active',
          clickable: true 
        }
      }
    };
  },
  computed: {
    swiper() {
      return this.$refs.mySwiper.swiper;
    }
  }
};
</script>
<style >
.custom .swiper-container{
  position: relative;
  width: 1280px;
  height: 458px;
  background-color: #f8f8f8;
}  
.custom .swiper-container .swiper-slide{
  text-align: center;
}
img {
  margin: 10px;
  border: 1px solid #e7e7e7;
}
.my-bullet{
  width: 32px; 
  height: 4px; 
  display: inline-block; 
  background: #afb2bb; 
  opacity: .2; 
  margin: 0 5px; 
}
.my-bullet-active{
  opacity: 1;
  background-color: #f97374;
}
</style>
<template>
    <main>
        <div class="wrapper">
            <swiper :navigation="true" :modules="modules">
                <swiper-slide><img src="./img/slide2.jpg" alt="err"></swiper-slide>
                <swiper-slide><img src="./img/slide3.jpg" alt="err"></swiper-slide>
                <swiper-slide><img src="./img/slide4.jpg" alt="err"></swiper-slide>
            </swiper>
        </div>
    </main>
</template>
<script >
  import { Swiper, SwiperSlide } from 'swiper/vue';

import 'swiper/css';

import 'swiper/css/navigation';
import { Navigation } from 'swiper/modules';

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Navigation],
    };
  },
};
</script>
<style src="./style.css">

</style>
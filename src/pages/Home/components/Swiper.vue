<template>
  <div class="wrapper">
    <swiper :options="swiperOption">
      <swiper-slide v-for="list of swipeLists" :key="list.id">
        <img :src="list.imgUrl" />
      </swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </div>
</template>


<script>
export default {
  name: "HomeSwiper",
  data() {
    return {
      swiperOption: {
        pagination: ".swiper-pagination",
        loop: true
      },
      swipeLists: [
        {
          id: "0001",
          imgUrl:
            "//dimg04.c-ctrip.com/images/70061a0000019887j7064_750_788_391.jpg"
        },
        {
          id: "0002",
          imgUrl:
            "//dimg04.c-ctrip.com/images/700416000000zfvklE101_750_788_391.jpg"
        }
      ]
    };
  }
};
</script>

<style scoped>
.wrapper >>> .swiper-pagination-bullet-active {
  background-color: #fff;
}
img {
  width: 100%;
  height: 150px;
  object-fit: cover;
}
</style>
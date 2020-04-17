<template>
  <div class="swiper">
    <div class="swiper-container">
      <el-carousel :interval="4000" type="card" height="280px">
        <el-carousel-item v-for="(item, index) in swiperList" :key="index">
          <img class="img" :src="item.picImg"/>
        </el-carousel-item>
      </el-carousel>
    </div>
  </div>
</template>

<script>
export default {
  name: "swiper",
  data() {
    return {
      swiperList: [
        {
          picImg: require("@/assets/img/swiper/1.jpg")
        },
        {
          picImg: require("@/assets/img/swiper/2.jpg")
        },
        {
          picImg: require("@/assets/img/swiper/3.jpg")
        },
        {
          picImg: require("@/assets/img/swiper/4.jpg")
        },
        {
          picImg: require("@/assets/img/swiper/5.jpg")
        }
      ]
    };
  }
};
</script>

<style scoped>
.swiper {
  width: 60%;
  margin: 40px auto;
}
.el-carousel__item:nth-child(2n) {
  background-color: #99a9bf;
}

.el-carousel__item:nth-child(2n + 1) {
  background-color: #d3dce6;
}
.img{
width:100%;
}
</style>

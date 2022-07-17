<template>
  <div class="">
    <div class="carousel-wrapper">
      <div>
        <div class="swiper-wrapper">
          <div
            class="img-wrapper swiper-slide relative"
            style="background: url('/agrosanzt-cerro-verde.jpg')"
          >
          <div class="swiper-slide__overlay"></div>
            <div class="swiper-slide__content">
              <h2>Agrosanzt</h2>
              <h3>Tu aliado de jardinería</h3>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      options: {
        slidesPerView: 1,
        loop: true,
      },
    }
  },
}
</script>
<style lang="scss" scoped>
.carousel-wrapper {
  width: 100%;
  .swiper-slide {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
    width: 100%;
    height: 70vh;
    position: relative;
    @media(max-width:750px){
      background-position: right !important;
    }
    & h2,h3{
    color:#ffffff;
    }
    & h2{
      font-size: 45px;
      font-weight: 700;
    }
    &__content {
      position: absolute;
      left: 10%;
    }
    &__overlay{
      width: 100%;
      height: 100%;
      position: absolute;
      background-color: rgba(0,0,0,0.5);
    }
  }
  .img-wrapper img {
    margin: auto;
    width: 100%;
    height: 70vh;
    background-image: linear-gradient(gray 100%, transparent 0);
    background-size: cover;
  }
}
</style>
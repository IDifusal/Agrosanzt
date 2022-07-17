<template>
<section class="overflow-hidden">
        <div class="banner-jar">
        <div class="grid grid-cols-1 md:grid-cols-2">
            <div></div>
            <div class="text-2xl md:text-4xl font-bold text-white w-2/3 md:w-full pl-5 md:pl-0">Jardines verticales en Arequipa</div>
        </div>
    </div>
</section>
</template>
<style scoped>
.banner-jar{
    padding: 200px 0px;
    background:url("~/assets/Agrosanzt-jardines-verticales-en-arequipa-peru.jpg"),rgba(5, 99, 71, 1);
      background-blend-mode: overlay;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
      animation: 60s ease 0s normal none infinite running zoomEffect;
  -webkit-animation: 60s ease 0s normal none infinite running zoomEffect;
  -o-animation: 60s ease 0s normal none infinite running zoomEffect;
  -moz--o-animation: 60s ease 0s normal none infinite running zoomEffect;
}
@keyframes zoomEffect {
    0% {transform: scale(1, 1)}
    50% {transform: scale(1.2, 1.2)}
    100% {transform: scale(1, 1)}
}
</style>
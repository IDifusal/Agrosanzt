<template>
  <section id="servicios" class="products py-20 container m-auto text-center">
    <h2 class="font-bold">Servicios</h2>
    <p>
      Para ofrecer un servicio de calidad contamos con un equipo calificado y un
      compromiso firme con la ecología.
    </p>
    <div class="">
      <div
        v-for="(item, index) in products"
        :key="index"
        class="products__item flex"
        :class="(index + 1) % 2 == 0 ? 'odd' : 'even'"
      >
        <div class="products__item mt-5 p-5 md:w-1/2">
          <h3 class="text-1xl font-bold" v-html="item.title"></h3>
          <p class="mt-3">{{ item.description }}</p>
        </div>
        <div class="md:w-1/2"></div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  data() {
    return {
      products: [
        {
          title: 'Instalación y mantenimiento de jardines verticales',
          description:
            'Se trata de una instalación vertical cubierta de plantas de distintas especies que no necesitan suelo para crecer. Diseñado con plantas naturales que pueden desarrollarse en barrancos y acantilados o pueden ser artificiales. Una vez instalado el jardín vertical, será necesario labores de mantenimiento como en toda área verde para que se encuentre sano y presente un estado saludable de acuerdo a cada estación del año.',
        },
        {
          title: 'Instalación y mantenimiento de <br>arte topiario',
          description:
            'El arte de la topiaria consiste en dar formas artísticas a las plantas mediante el recorte típicamente en arbustos y árboles de hoja perenne en formas intrincadas o estilizadas con tijeras de podar. Estas formas pueden representar animales, objetos, espirales, entre otras; es un tipo de escultura viviente. Su principal objetivo es la representación estética pero también es una excelente manera de agregar volumen y perspectiva a su jardín.',
        },
      ],
    }
  },
}
</script>
<style lang="scss" scoped>
.products__item {
  &.odd {
    flex-direction: row-reverse;
  }
}
</style>
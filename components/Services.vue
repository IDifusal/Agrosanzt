<template>
    <section id="servicios" class="products py-20 container m-auto text-center">
      <h2 class="font-bold">Servicios</h2>
      <p>Sunt in amet ex veniam et exercitation ea pariatur enim non consequat Lorem sit in.</p>
      <div class="grid grid-cols-1 md:grid-cols-4">
        <div
          v-for="(item, index) in products"
          :key="index"
          class="products__item"
        >
          <div class="products__item mt-5 p-5">
            <h2 class="text-2xl font-bold">{{ item.title }}</h2>
            <p class="mt-3">{{ item.description }}</p>
          </div>
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
          title: 'Jardines Verticales',
          description:
            'Ex ex laborum sit ipsum dolore. Est elit Lorem aute nisi amet Lorem ea incididunt. Quis occaecat sit et aute sit aliquip eu est laborum excepteur anim Lorem laborum eu.',
        },
        {
          title: 'Jardines Verticales',
          description:
            'Ex ex laborum sit ipsum dolore. Est elit Lorem aute nisi amet Lorem ea incididunt. Quis occaecat sit et aute sit aliquip eu est laborum excepteur anim Lorem laborum eu.',
        },
        {
          title: 'Jardines Verticales',
          description:
            'Ex ex laborum sit ipsum dolore. Est elit Lorem aute nisi amet Lorem ea incididunt. Quis occaecat sit et aute sit aliquip eu est laborum excepteur anim Lorem laborum eu.',
        },
        {
          title: 'Jardines Verticales',
          description:
            'Ex ex laborum sit ipsum dolore. Est elit Lorem aute nisi amet Lorem ea incididunt. Quis occaecat sit et aute sit aliquip eu est laborum excepteur anim Lorem laborum eu.',
        },
      ],
    }
  },
}
</script>
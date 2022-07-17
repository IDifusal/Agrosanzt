<template>
  <div >
    <div class="container m-auto pt-20">
      <h1 class="text-center text-4xl font-bold">
        Agrosanzt, soluciones en jardinería
      </h1>
      <p class="text-center mt-4 mt-10">
        Aliquip aliqua voluptate sit Lorem dolor non nisi pariatur. Est qui
        Lorem voluptate ex laborum ipsum Lorem dolore consectetur. Quis qui
        exercitation duis officia ipsum do eu anim sint elit ex ipsum. Ut
        incididunt nostrud adipisicing cupidatat tempor enim id veniam Lorem
        quis labore consectetur duis. Occaecat ad amet id mollit ea ad veniam ex
        eiusmod labore est eu dolor adipisicing. Ea cupidatat proident ut mollit
        ullamco eiusmod. Laborum velit consectetur amet proident exercitation
        irure duis sunt sunt velit non dolore officia laboris.
      </p>
      <img
        src="/agrosanzt-trabajos.jpg"
        class="m-auto mt-5 w-1/2 rounded"
        alt="Agrosanzt, soluciones en jardinería"
      />
    </div>
    <section id="productos" class="products py-20 container m-auto">
      <h2 class="text-center font-bold">Productos</h2>
      <p class="text-center">
        Sunt in amet ex veniam et exercitation ea pariatur enim non consequat
        Lorem sit in.
      </p>
      <div class="grid grid-cols-1 md:grid-cols-2 pt-5">
        <div
          v-for="(item, index) in products"
          :key="index"
          class="products__item p-5 flex"
        >
        <div class="w-1/3 md:mr-5">
        <img :src="require(`~/assets/images/agrosanzt${index+1}.jpg`)" :alt="item.title"  class="ml-auto md:w-1/2">
        </div>
          <div class="w-2/3">
            <h3 class="font-bold">{{ item.title }}</h3>
            <p>{{ item.description }}</p>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>
<script>
export default {
  data() {
    return {
      products: [
        {
          title: 'Abono',
          description:
            'Ex ex laborum sit ipsum dolore. Est elit Lorem aute nisi amet Lorem ea incididunt. Quis occaecat sit et aute sit aliquip eu est laborum excepteur anim Lorem laborum eu.',
        },
        {
          title: 'Abono',
          description:
            'Ex ex laborum sit ipsum dolore. Est elit Lorem aute nisi amet Lorem ea incididunt. Quis occaecat sit et aute sit aliquip eu est laborum excepteur anim Lorem laborum eu.',
        },
        {
          title: 'Abono',
          description:
            'Ex ex laborum sit ipsum dolore. Est elit Lorem aute nisi amet Lorem ea incididunt. Quis occaecat sit et aute sit aliquip eu est laborum excepteur anim Lorem laborum eu.',
        },
        {
          title: 'Abono',
          description:
            'Ex ex laborum sit ipsum dolore. Est elit Lorem aute nisi amet Lorem ea incididunt. Quis occaecat sit et aute sit aliquip eu est laborum excepteur anim Lorem laborum eu.',
        },
        {
          title: 'Abono',
          description:
            'Ex ex laborum sit ipsum dolore. Est elit Lorem aute nisi amet Lorem ea incididunt. Quis occaecat sit et aute sit aliquip eu est laborum excepteur anim Lorem laborum eu.',
        },
        {
          title: 'Abono',
          description:
            'Ex ex laborum sit ipsum dolore. Est elit Lorem aute nisi amet Lorem ea incididunt. Quis occaecat sit et aute sit aliquip eu est laborum excepteur anim Lorem laborum eu.',
        },
        {
          title: 'Abono',
          description:
            'Ex ex laborum sit ipsum dolore. Est elit Lorem aute nisi amet Lorem ea incididunt. Quis occaecat sit et aute sit aliquip eu est laborum excepteur anim Lorem laborum eu.',
        },
        {
          title: 'Abono',
          description:
            'Ex ex laborum sit ipsum dolore. Est elit Lorem aute nisi amet Lorem ea incididunt. Quis occaecat sit et aute sit aliquip eu est laborum excepteur anim Lorem laborum eu.',
        },
      ],
    }
  },
}
</script>
<template>
  <div>
    <div class="container m-auto pt-20">
      <h1 class="text-center text-4xl font-bold">
        Agrosanzt, soluciones en jardinería
      </h1>
      <p class="text-center mt-4 mt-10">
        Un jardín bien cuidado da una mejor apariencia a su empresa. Por eso
        Agrosanzt ofrece servicio de jardinería a sus clientes. El mantenimiento
        de jardines es necesario para mejorar su aspecto, así como también, para
        que los árboles, plantas y flores crezcan sanos y fuertes. Las plantas
        requieren unas series de nutrientes para desarrollarse bien, florecer en
        cantidad y calidad, resistir el calor y el frio para lo cual la tierra
        necesita ser enriquecida de forma regular mediante el aporte de abonos
        orgánicos. <br /><br />El cuidado de las plantas representa mucho más
        que solo regarlas de vez en cuando. Uno de los cuidados más importantes
        que tenemos que procurar es la protección contra las plagas. Por lo
        tanto, es importante fumigar con productos adecuados que actuaran como
        protectores contra plagas.
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
        Contamos con una variedad de productos los cuales están dirigidos al
        rubro de la jardinería.
      </p>
      <div class="grid grid-cols-1 md:grid-cols-2 pt-5">
        <div
          v-for="(item, index) in products"
          :key="index"
          class="products__item p-5 flex"
        >
          <div class="w-1/3 md:mr-5">
            <img
              :src="require(`~/assets/images/agrosanzt${index + 1}.jpg`)"
              :alt="item.title"
              class="ml-auto md:w-1/2"
            />
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
          title: 'Compost',
          description:
            'Es un fertilizante orgánico totalmente natural y sirve como medio para la descomposición total o parcial de residuos tóxicos en plantas. Puede obtenerse de desechos de la cocina y jardín.',
        },
        {
          title: 'Humus de Lombis',
          description:
            'Es un abono natural con gran porcentaje de nutrientes generado a partir del estiércol de las lombrices. Tiene una estructura grumosa y esponjosa que facilita la aireación y la retención de agua, libre de semillas activas u hongos.',
        },
        {
          title: 'Piedra Pomez',
          description:
            'Ayuda a que el suelo se encuentre menos compactado, más ligero; así favorece la circulación del agua, abono y el enraizamiento de la planta. Es rica en nutrientes, no afecta el equilibrio del suelo y existe una reducción de riego.',
        },
        {
          title: 'Musgo',
          description:
            'EAyuda a mantener la humedad en el suelo, esto previene erosiones y mejora la captación de agua y la germinación de semillas de otras plantas.',
        },
        {
          title: 'Cascarilla de Arrox',
          description:
            'Posee una fuente rica en sílice lo que favorece a vegetales dándoles mayor resistencia contra insectos y microorganismos. Reduce la presencia de malezas, disminuye la temperatura del suelo y un adecuado crecimiento.',
        },
        {
          title: 'Tierra Vegetal',
          description:
            'Es un sustrato óptimo para la realización de cualquier tipo de plantación en el jardín, contiene una mezcla de compost vegetal, arena y tierra natural, además de materias orgánicas en diversos grados de descomposición.',
        },
        {
          title: 'Biochar',
          description:
            'Es el carbón obtenido a partir de materia orgánica de restos vegetales tras someterla a pirólisis controlada en ausencia de oxígeno. Brinda una mayor capacidad de retención de minerales y la disposición de fósforo en el suelo.',
        },
        {
          title: 'Tierra Preparada',
          description:
            'Es un sustrato utilizado para mejorar el crecimiento de todo tipo de plantas ornamentales que colocas en macetas, jardineras, macizos y otros, ya que tienen un buen drenaje de agua. Está compuesta por musgo, tierra vegetal, tierra de chacra y fertilizantes sintéticos.',
        },
        {
          title: 'Sustrato Preparado',
          description:
            'Es una mezcla preparada, lista para sembrar o para trasplantar, está compuesto por material vegetal compostado, fibra de coco, materia orgánica, turba rubia y negra, fertilizante, además de activador de raíces.',
        },
        {
          title: 'Bonsai',
          description:
            'Es una planta que se mantiene pequeña dándole forma, podando el tronco, las hojas y las raíces cada cierto tiempo, dependiendo de la especie.',
        },
      ],
    }
  },
}
</script>
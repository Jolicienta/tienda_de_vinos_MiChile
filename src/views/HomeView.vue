<template>
    <v-carousel>
      <v-carousel-item
        v-for="(item,i) in items"
        :key="i"
        :src="item.src"
        reverse-transition="fade-transition"
        transition="fade-transition"
      ></v-carousel-item>
    </v-carousel>

</template>

<script>
  import HelloWorld from '../components/HelloWorld'

  export default {
    name: 'Home',

    data () {
          return {
            items: [
              {
                src: 'https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg',
              },
              {
                src: 'https://cdn.vuetifyjs.com/images/carousel/sky.jpg',
              },
              {
                src: 'https://cdn.vuetifyjs.com/images/carousel/bird.jpg',
              },
              {
                src: 'https://cdn.vuetifyjs.com/images/carousel/planet.jpg',
              },
            ],
          }
        },
        
    components: {
      HelloWorld,
    },
  }
</script>

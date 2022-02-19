<template>
  <hello-world />
</template>

<script>
  import HelloWorld from '../components/HelloWorld'

  export default {
    name: 'Home',

    components: {
      HelloWorld,
    },
    data: () => ({
      categories : [
      { 
        id: 1,
        image: 'https://via.placeholder.com/150',
        name: 'Ekonomi',
        slug: 'ekonomi'
      },
      { 
        id: 2,
        image: 'https://via.placeholder.com/150',
        name: 'Agama',
        slug: 'agama'
      },    
      ]
    })
  }
</script>

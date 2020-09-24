<template>
  <header>
      <img :src="image">
  </header>
</template>
worm
<script>
export default {
    name: 'Header',         //component name - required
    data() {            
        return {
            image: require('@/assets/logo.png')             //sourcefolder/assets/
        };
    }                      
};
</script>

<style scoped>
    img {
        width: 300px;
    }

    @media(max-width: 700px) {
        img {
            display: block;
            margin: auto;
        }
    }
</style>
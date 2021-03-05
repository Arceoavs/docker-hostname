<template lang="pug">
.home
  h1 What´s my hostname?
  h2 Full URL: 
  p {{currentUrl}}
  h2 Host:
  p {{host}}
</template>

<script>
export default {
  name: 'Home',
  components: {},
  data() {
    return {
      currentUrl: location.toString(),
      host: location.host
    };
  }
};
</script>

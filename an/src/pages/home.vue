<template>
  <div class="home">
    {{changeimg_big}}
  </div>
</template>

<script>
import { mapGetters } from 'vuex';

export default {
  name: 'home',
  data () {
    return {
      changeimg_big:''
    }
  },
  computed:{

  },
  created() {
    this.changeimg_big = this.$store.state.an;
  }
}
</script>

<style scoped lang="scss">

</style>

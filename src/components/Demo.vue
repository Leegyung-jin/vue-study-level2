<template>
  <div id="root">
<!--    <p>{{ this.$store.getters.originalPrice }}</p>-->
<!--    <p>{{ this.$store.getters.doublePrice }}</p>-->
<!--    <p>{{ this.$store.getters.triplePrice }}</p>-->
    <p>{{ originalPrice }}</p>
    <p>{{ doublePrice }}</p>
    <p>{{ triplePrice }}</p>
  </div>
</template>

<script>
import { mapGetters } from 'vuex'

export default {
  computed: {
    // originalPrice(state) {
    //   return this.$store.getters.originalPrice;
    // },
    // doublePrice(state) {
    //   return this.$store.getters.doublePrice;
    // },
    // triplePrice(state) {
    //   return this.$store.getters.triplePrice;
    // }
    // 헬퍼 함수를 이용해서 간단하게 표현할 수 있다.
    ...mapGetters(['originalPrice', 'doublePrice', 'triplePrice'])
  }
}
</script>

<style scoped>

</style>
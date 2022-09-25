<template>
  <ul>
    <li v-for="item in limit" v-show="!(item % 2)" :key="item">
        {{ base }} x {{ item }} = {{ base * item }}
    </li>
  </ul>
</template>

<script>
export default {
  name: "Multiplica-items",
  data() {
    return {
      base: 2,
      limit: 10
    }
  }
}
</script>

<style scoped>

</style>
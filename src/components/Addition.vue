<template>
  <div>
    <h3>当前最新的count值为：{{this.$store.state.count}}</h3>
    <button @click="btnHandler1">+1</button>
    <button @click="btnHandler2">+3</button>
  </div>
</template>

<script>
export default {
  date() {
    return {}
  },
  methods: {
    btnHandler1() {
      this.$store.commit('add')
    },
    btnHandler2() {
      this.$store.commit('addN',3)
    }
  }
}
</script>

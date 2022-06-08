<template>
  <InputText type="text" :modelValue="value1" @blur="sayHi" />
  <span :style="{marginLeft: '.5em'}">{{ value1 }}</span>
</template>

<script>
import InputText from 'primevue/inputtext'
export default {
  name: 'App',
  components: {
    InputText,
  },
  data() {
    return {
      value1: '',
    }
  },
  methods: {
    sayHi(e) {
      console.log(e)
    },
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

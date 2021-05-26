<template>
  <b-container>
    <b-row>
      <b-col cols="4" lg="6">Hello</b-col>
      <b-col cols="8" lg="6">World</b-col>
    </b-row>

    Счётчик: {{ $store.state.counter.counter }}
    <b-btn v-on:click="$store.commit('counter/increment')">Добавить</b-btn>
    <b-btn v-on:click="$store.commit('counter/decrement')">Убавить</b-btn>
  </b-container>
</template>

<script>
export default {}
</script>

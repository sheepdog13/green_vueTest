<script>
export default {
  data() {
    return {
      count: 0,
      titleClass : "title"
    }
  },
  methods: {
    increment() {
      this.count++
    }
  }
}
</script>

<template>
  <h1 :class="titleClass">{{count}}</h1>
  <h2>vue로 확인하는 웹페이지 입니다. 아래버튼을 누르면 값이 1씩증가합니다</h2>
  <button v-on:click="increment">1+</button>
</template>

<style>
  .title {color: red;}
</style>
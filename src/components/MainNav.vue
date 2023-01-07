<template>
<!--<h1>aaa</h1>-->
<!--  <h2>{{objectOfAttrs}}</h2>-->
<!--  <div v-bind="objectOfAttrs"></div>-->
<!--  <h1>{{ ok ? 'YES' : 'NO' }}</h1>-->
  <h1>{{ count }}</h1>
  <div>
    <button v-on:click="increment(2)">click</button>

  </div>
  <div v-bind="objectOfAttrs">sss</div>

</template>

<script>
export default {
  name: "MainNav",
  data() {
    return {
      objectOfAttrs: {
        id: 'container',
        class: 'wrapper'
      },
      count: 0
    }
  },

  // actions
  methods: {
    increment(data) {
      this.count = this.count + data;
    }
  }

}


</script>

<style scoped>
h1 {
  color: #222222;
  font-size: 25px;
}
</style>



<template>
  <div id="app" v-bind:class="color">
    <p v-on:click="change"><a :href="link">{{message}}</a></p>
    <input type="text" v-model="message"/>
  </div>
</template>

<script>
export default {
  name: 'app',
    data () {
    return {
        message: "Hello",
        color: "white",
        link: "https://www.google.com"
    }
  },
  methods: {
    change() {
        if (this.color === "white") {
            return this.color = "green"
        } else {
            return this.color = "white";
        }
    }
  }
}
</script>

<style>
  .green {
    background-color: green;
  }
  .red {
    background-color: red;
  }
  .white {
    background-color: white;
  }
</style>

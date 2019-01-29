<template>
  <div id="app">
    <ul>
      <li v-for="item in message">{{item}}</li>
    </ul>
    <input type="text" v-model="message"/>
  </div>
</template>

<script>
export default {
  name: 'app',
    data () {
    return {
        message: ""
    }
  },
  methods: {

  },
  computed: {
    test: function () {
        return this.message.split(',');
    }
  },
  watch: {
    "message": function () {
      
    }
  }
}
</script>

<style>

</style>

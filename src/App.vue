<template>
  <div class="container">
    <div class="row">
      <div class="col text-center">
        <h1>Reverse</h1>
      </div>
    </div>

    <div class="row">
      <div class="col-md-6">
        <h4>String</h4>
        <input type="text" v-model="string">
      </div>
      <div class="col-md-6">
        <h4>Reversed String</h4>
        <div>
          {{ reverseString }}
        </div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'app',
  data() {
    return {
      string: ''
    }
  },
  computed: {
    reverseString: function() {
      return this.string.split('').reverse().join('')
    }
  }
}
</script>

<style>

</style>

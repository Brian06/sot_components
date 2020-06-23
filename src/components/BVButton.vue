<template>
  <button class="bv-button" v-on:click="toBV">
    {{ msg }}
  </button>
</template>

<script>
export default {
  name: 'BV_Button',
  props: {
    msg: String,
    user: String,
  },
  methods: {
    toBV: function () {
      alert(`Bye ${this.user}!`);
      window.location = 'https://www.beenverified.com';
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .bv-button {
    background: #81B44C;
    color: #FFF;
    border-radius: 6px;
    font-family: 'Lato', sans-serif;
    font-weight: bold;
    font-size: 26px;
    border: 0;
    cursor: pointer;
    width: 180px;
    height: 70px;
    transition: all 0.25s ease-out;
  }

  .bv-button:hover {
    background: #638A3A;
    text-decoration: none;
  }
</style>
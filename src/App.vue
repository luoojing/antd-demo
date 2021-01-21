<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">

    <a-button type="danger" shape="circle">Button</a-button>
    <a-icon type="wifi"/>
        <a-radio-group v-model="size">
          <a-radio value="small">Small</a-radio>
          <a-radio value="middle">Middle</a-radio>
          <a-radio value="large">Large</a-radio>
        </a-radio-group>
        <br />
        <br />
        <a-space :size="size" direction="vertical">
          <a-button type="primary">Primary</a-button>
          <a-button>Default</a-button>
          <a-button type="dashed">Dashed</a-button>
          <a-button type="link">Link</a-button>
        </a-space>



  </div>

</template>

<script>
export default {
  data() {
    return {
      size: 'small',
    };
  },
};


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

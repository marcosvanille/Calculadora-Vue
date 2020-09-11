<template>
  <div id="app">
    <h1>Calculadora</h1>
    <Calculator/>
  </div>
</template>

<script>
import Calculator from "@/main/Calculator";

export default {
  components: {Calculator}
}
</script>

<style>
* {
  font-family: "Roboto Light", "monospace";
}

body {
  margin: 0;
}

#app {
  display: flex;
  flex-direction: column;
  height: 100vh;
  justify-content: center;
  align-items: center;
  text-align: center;

  color: #fff;
  background: linear-gradient(90deg, rgba(2, 0, 36, 1) 0%, rgba(9, 103, 121, 1) 88%, rgba(0, 212, 255, 1) 100%);

}


</style>
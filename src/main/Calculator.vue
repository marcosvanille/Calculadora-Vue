<template>
  <div class="calculator">
    <Display value="1000"/>
    <Button label="AC" triple @onCalcButtonClick="clearMemory"/>
    <Button label="/" operation @onCalcButtonClick="setOperation"/>
    <Button label="7" @onCalcButtonClick="addDigit"/>
    <Button label="8"/>
    <Button label="9"/>
    <Button label="*" operation/>
    <Button label="4"/>
    <Button label="5"/>
    <Button label="6"/>
    <Button label="-" operation/>
    <Button label="1"/>
    <Button label="2"/>
    <Button label="3"/>
    <Button label="+" operation/>
    <Button label="0" double/>
    <Button label="."/>
    <Button label="=" operation/>
  </div>
</template>

<script>
import Display from "@/components/Display"
import Button from "@/components/Button";

export default {
  components: {Button, Display},
  methods: {
    clearMemory() {
      console.log('limpar  Memoria!')
    },
    setOperation(operation) {
      console.log('Operaçao' + operation)
    },
    addDigit(n) {
      console.log('Digito' + n)
    }
  }
}
</script>

<style scoped>
.calculator {
  height: 320px;
  width: 235px;
  border-radius: 5px;
  overflow: hidden;

  display: grid;
  grid-template-columns:repeat(4, 25%);
  grid-template-rows: 1fr 48px 48px 48px 48px 48px;
}
</style>
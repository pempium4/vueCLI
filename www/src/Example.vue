<template>
  <div id="example">
    <h1>{{ greeting }}</h1>
    <app-input :msg="greeting"></app-input>
  </div>
</template>

<script>
import Input from "./Input";
export default {
  name: "Example",
  data: function (){
    return{
      greeting: 'Ex text'
    }
  },
  components: {
    'app-input' : Input
  }
}
</script>

<style scoped>

</style>

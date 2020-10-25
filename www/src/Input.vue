<template>
  <div>
    <h3>{{msg}}</h3>
    <input type="text" :value="msg" @input="changeMSG">
    <p>{{text}}</p>
  </div>
</template>

<script>
export default {
  data: function (){
    return{
      text: ''
    }
  },
  props: [
    'msg'
  ],
  methods: {
    changeMSG (event){
      this.msg = event.target.value;
    }
  }
}
</script>

<style scoped>

</style>

<template>
  <button value="click" @click="btnBus"></button>
</template>
<script>
import eventBus from '../store/eventBus';
export default{
  name:"TheWelcome",
 methods:{
  btnBus(){
    eventBus.emit('test', "ok");
  },
  data(){
    return{
      data : "Ok"
    }
  }
 }
}
</script>

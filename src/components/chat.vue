<template>
  <div id="chat" class="chat-style">
      <display></display>
      <userinput></userinput>
  </div>
</template>

<script>
import userinput from './user-input'
import display from './display'
export default {
    name:"chat",
    data(){

    },
    props:[],
    components:{
        userinput,display
    }
}
</script>

<style>
    .chat-style{
        width:500px;
        height:700px;
    }
</style>
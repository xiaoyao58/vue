<template>
  <div id="app" class="app-style">
    <userlist></userlist>
    <chat></chat>
  </div>
</template>

<script>
import chat from './components/chat'
import userlist from './components/userlist'
export default {
  name: 'App',
  components: {
    userlist,chat
  }
}
</script>

<style>
  .app-style{
    margin: 0 auto;
    display:flex;
    width:800px;
    height:700px;
    border:1px solid #ccc;
  }
</style>

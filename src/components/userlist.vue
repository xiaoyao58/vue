<template>
  <div id="user" class="list-style">
    <user v-for="(item,index) in users" :usermsg="item" :key="index"></user>
  </div>
</template>

<script>
import user from "./user";
export default {
  name: "User",
  data: function() {
    return {
      users: [
        {
          name: "逍遥",
          avatar: require("../assets/imgs/1.jpg"),
          msg: "hello 我是逍遥"
        },
        {
          name: "天依",
          avatar: require("../assets/imgs/2.jpg"),
          msg: "hello 我是天依"
        },
        {
          name: "希尔",
          avatar: require("../assets/imgs/3.jpg"),
          msg: "hello 我是希尔"
        }
      ]
    };
  },
  components: {
    user
  }
};
</script>

<style>
.list-style {
  width: 300px;
  height: 700px;
  background-color: gainsboro;
}
</style>
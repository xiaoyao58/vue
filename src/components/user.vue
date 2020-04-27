<template>
  <div id="user" class="user" :class="[{active:pitch},{mouse:true}]" @click="get_pitch">
    <img :src="usermsg.avatar" />

    <div>
      <h3>{{usermsg.name}}</h3>
      <p>{{usermsg.msg}}</p>
    </div>
  </div>
</template>

<script>
export default {
  props: ["usermsg"],
  data(){
      return {
          pitch:false,
      }
  },
  methods: {
      get_pitch(){
          this.pitch = !this.pitch;
      }
  }
};
</script>

<style>
.user {
  display: flex;
  height: 70px;
  background-color: white;
  /* border: 1px solid rgb(223, 212, 212); */
  padding: 10px;
}

.user img {
  left: 0;
  vertical-align: middlel;
  width: 60px;
  height: 70px;
  border-radius: 50%;
}

.user h3 {
  width: 239px;
  margin-top: 0px;
  margin-left: 50px;
}

.user p {
  width: 239px;
  font-size: smaller;
  color: gray;
  margin-top: 20px;
  margin-left: 30px;
}

.active{
    background-color:#ccc;
}

.mouse:hover{
    background-color:#ccc;
}
</style>
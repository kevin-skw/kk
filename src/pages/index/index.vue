<template>
  <div>
    <div class="seach"> 
       <input type="text" :class="{feach:feach}" @click="seach()">
       <p class="cancet" @click="quxiao()" >取消</p>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      feach :false
    }
  },

  methods: {
    seach(){
      console.log(110)
      this.feach = true;
    },
    quxiao(){
      console.log(220)
      this.feach = false;
    }
  }
}
</script>

<style scoped  >

.seach{
  height: 60rpx;
  background:#ea4451;
 
}
.feach{
  display: flex;
  height: 60rpx;
  background: pink;
  /*position: absolute;*/
  /*margin: 0 80rpx 0 0;*/
}
input{
  flex: 1;
  width: 80%;
  background: #ffffff;
  border-radius: 10rpx;
}
.cancet{
  width: 80rpx;
  height: 60rpx;
  line-height: 60rpx;
  font-size: 30rpx;
  /*position: relative;
  left: 600rpx;*/
  display: none;
}
</style>
<template>
  <div id="app" >
    <Slider @deleteItem="deleteItem(1)">
      <div class="box www"></div>
    </Slider>
    <br>
    <Slider  @deleteItem="deleteItem(2)">
      <div class="box  zzz"></div>
    </Slider>
  </div>
</template>

<script>

import Slider from './components/slider/index'
export default {
  name: 'app',
  components: {
    Slider
  },
  methods:{
    deleteItem(i){
      alert(i)
    }
  }
}
</script>

<style lang="less">
*{
  margin: 0;
  padding: 0;
}
#app {
  overflow: hidden;
}
.box {
  width: 100%;
  height: 50px;
  background-color: aquamarine;
}
.cont  {
  width: 100%;
  height: 50px;
  background-color: gray;
}
</style>

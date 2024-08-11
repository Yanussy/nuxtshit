<template>

     <div class="canvas-container">
    <canvas ref="myCanvas" width="1000" height="1000"></canvas>
  </div>

 </template>

<script>
export default {
  name: 'game',
  mounted(){
    const canvas = this.$refs.myCanvas;
    const context = canvas.getContext('2d');
    context.fillStyle = 'black';
    context.fillRect(0,0,300,200);
  }
};

</script>

<style scoped>
.game {
  padding: 20px;
  background-color: #f0f0f0;
  border-radius: 8px;
  text-align: center;
}
</style>

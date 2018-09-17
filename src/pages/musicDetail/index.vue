<template>
    <div class="main">
      <div class="circle-author">

      </div>
    </div>
</template>

<script>
  export default {
    name: "index"
  };
</script>

<style scoped>
  .main {
    background: -webkit-linear-gradient(#282828,gray);
    position: fixed;
    height: 100%;
    width: 100%;
    display:flex;
    /*flex-direction:column; !*纵向显示*!*/
    /*align-items:center;!*垂直居中*!*/
    /*justify-content: center;!*水平居中*!*/
    opacity: 0.8;
    text-align: center;
  }
  .circle-author {
    background: #586c94;
    width: 100px;
    height: 100px;
    justify-content: center;/*水平居中*/
    display: flex;
  }
</style>

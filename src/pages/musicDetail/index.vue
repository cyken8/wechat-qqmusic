<template>
    <div class="main">
      <div class="header">
        <img src="../../../static/icon/music/backpage.png" style="width: 20px;height: 20px" class="header-back">
        <div>

        </div>
      </div>
      <div class="tag">
        <div class="tag-item">
            标准
        </div>
        <div class="tag-item">
            音效
        </div>
      </div>
      <div class="circle-author">
        <div class="circle-image"></div>
      </div>
      <div class="detail">{{musicDetail}}</div>
      <div class="cate">
        <div class="cate-item">
          <div class="cate-item-circle" style="background: #d5d5d6"></div>
        </div>
        <div class="cate-item">
          <div class="cate-item-circle" style="background: #ffffff"></div>
        </div>
        <div class="cate-item">
          <div class="cate-item-circle" style="background: #d5d5d6"></div>
        </div>
      </div>
      <div class="footer-progress">
        <slider block-size="18" style="width: 70%"></slider>
      </div>
      <div class="footer-play">
        <div class="footer-play-item">
          <img src="../../../static/icon/music/single.png" style="width: 20px;height: 20px">
        </div>
        <div class="footer-play-item">
          <div>
            <img src="../../../static/icon/music/back.png" style="width: 30px;height: 30px">
          </div>
        </div>
        <div class="footer-play-item">
          <div>
            <img src="../../../static/icon/music/play.png" style="width: 40px;height: 40px">
          </div>
        </div>
        <div class="footer-play-item">
          <div>
            <img src="../../../static/icon/music/next.png" style="width: 30px;height: 30px">
          </div>
        </div>
        <div class="footer-play-item">
          <img src="../../../static/icon/music/single.png" style="width: 20px;height: 20px">
        </div>
      </div>
      <div class="footer-operation">
        <div class="footer-operation-item">
          <img src="../../../static/icon/music/like-before.png" style="width:20px;height: 20px">
        </div>
        <div class="footer-operation-item">
          <img src="../../../static/icon/music/download.png" style="width:20px;height: 20px">
        </div>
        <div class="footer-operation-item">
          <img src="../../../static/icon/music/share.png" style="width:20px;height: 20px">
        </div>
        <div class="footer-operation-item">
          <img src="../../../static/icon/music/comments.png" style="width:20px;height: 20px">
        </div>
      </div>
    </div>
</template>

<script>
  export default {
    name: "index",
    data: {
      musicDetail: '书香年华 - 许嵩 （Vae Xu）/孙涛'
    }
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
    justify-content: center;/*水平居中*/
    opacity: 0.8;
    text-align: center;
    color: white;
  }
  .header {
    display: flex;
    flex-direction: column;
    position: fixed;
    top: 5px;
    width: 100%;
    height: 50px;
    background: #e64340;
    justify-content: center;
  }
  .header-back {
    position: fixed;
    left: 15px;
    top: 10px;
  }
  .header-title {

  }
  .tag {
    position: fixed;
    top: 70px;
    width: 50%;
    height: 40px;
    display: flex;
  }
  .tag-item {
    flex: 1;
    border: 3px solid #ffffff;
    -webkit-border-radius: 7px;
    margin: 3px;
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
    font-size: 17px;
  }
  .tag-item-button {
    border: 3px solid #ffffff;
    -webkit-border-radius: 7px;
    margin: 3px;
  }
  .circle-author {
    background: black;
    width: 200px;
    height: 200px;
    display: flex;
    -webkit-border-radius: 100px;
    margin-top: 130px;
    justify-content: center;
    align-items: center;
  }
  .circle-image {
    background: #d9d9d9;
    width: 190px;
    height: 190px;
    display: flex;
    -webkit-border-radius: 95px;
  }
  .detail {
    position: fixed;
    width: 80%;
    bottom: 220px;
    height: 20px;
    font-size: 17px;
  }
  .cate {
    width: 70px;
    height: 30px;
    position: fixed;
    display: flex;
    justify-content: center;
    /*background: #586c94;*/
    bottom: 180px;
    align-items: center;
  }
  .cate-item {
    flex: 1;
    display: flex;
    justify-content: center;
  }
  .cate-item-circle {
    height: 10px;
    width: 10px;
    -webkit-border-radius: 5px
  }
  .footer-play-circle {
    -webkit-border-radius: 18px;
    border: 3px solid white;
    width: 36px;
    height: 36px;
  }
  .footer-progress {
    position: fixed;
    bottom: 130px;
    width: 100%;
    /*background: #e64340;*/
    height: 60px;
    justify-content: center;
    display: flex;
    align-items: center;
  }
  .footer-play {
    display: flex;
    position: fixed;
    /*background: #e64340;*/
    height: 80px;
    bottom: 50px;
    width: 100%;
    align-items: center;
  }
  .footer-play-item {
    flex: 1;
    justify-content: center;
    align-items: center;
    display: flex;
  }
  .footer-play-items {
    flex: 1;
    /*border: 3px solid #FFFFFF;*/
    /*-webkit-border-radius: 6px;*/
  }
  .footer-operation {
    display: flex;
    height: 50px;
    width: 100%;
    position: fixed;
    bottom: 0;
    align-items: center;
  }
  .footer-operation-item {
    flex: 1
  }
</style>

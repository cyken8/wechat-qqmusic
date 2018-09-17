<template>
    <div @click="expandDetail">
      <div class="audio">
        <!--<audio poster='http://y.gtimg.cn/music/photo_new/T002R300x300M000003rsKF44GyaSk.jpg?max_age=2592000' name="此时此刻" id="myAudio"-->
        <!--author="许巍" src='http://ws.stream.qqmusic.qq.com/M500001VfvsJ21xFqb.mp3?guid=ffffffff82def4af4b12b3cd9337d5e7&uin=346897220&vkey=6292F51E1E384E06DCBDC9AB7C49FD713D632D313AC4858BACB8DDD29067D3C601481D36E62053BF8DFEAF74C0A5CCFADD6471160CAF3E6A&fromtag=46'-->
        <!--controls loop></audio>-->
        <div style="line-height: 80px;margin-left: 10px">
          <img src="http://y.gtimg.cn/music/photo_new/T002R300x300M000003rsKF44GyaSk.jpg?max_age=2592000" style="width:40px;height: 40px;border-radius: 20px;border:1px solid">
        </div>
        <div style="margin-left: 15px;margin-top: 6px">
          <div style="text-align: left;font-size: 15px">此时此刻</div>
          <div style="text-align: left;color:#acacac;font-size:12px">许巍</div>
        </div>
        <div style="margin-left: 110px;">
          <canvas canvas-id="playRate" style="width: 30px;height: 30px;"></canvas>
        </div>
        <div style="line-height: 70px;float:right;margin-left: 10px">
          <img src="/static/icon/musicList.png" style="width: 30px;height: 30px"/>
        </div>
      </div>
    </div>
</template>

<script>
  export default {
    name: "music",
    methods: {
      expandDetail: function() {
        wx.navigateTo({
          url: '../../pages/musicDetail/main',
          success: function() {
            console.log('success')
          },
          fail: function() {
            console.log('fail')
          }
        })
      }
    }
  };
</script>

<style scoped>
  .audio {
    width: 100%;
    background: white;
    height: 60px;
    position: fixed;
    bottom: 0;
    border: 1px solid #f5f5f5;
    display: flex;
    z-index: 99;
  }
</style>

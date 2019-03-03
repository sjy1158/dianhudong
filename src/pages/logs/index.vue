<template>
  <div>
    <div class="headerbg">
      <img src="/static/home/banner.png" alt="">
    </div>

    <div style="position: relative;width: 100%;z-index: 9999">
      <div class="title">
        <div class="headertext"></div>
      </div>
    </div>

    <div class="time" style="position: relative">
      <div class="timecontent">
        <div class="alltime">
          <img src="/static/home/item1.png" alt="">
          <span class="huiyuan">月卡会员</span>
          <span style="float: right;margin-right: 40px;" class="daoqi">2019年2月20日到期</span>
        </div>
      </div>
    </div>

    <div style="width: 100%;height: 46px;line-height: 46px;letter-spacing: 2px;font-size: 14px;color: #000000;padding-left: 30px;">商家服务</div>

    <div class="items">
      <ul>
        <li>
          <img src="/static/my/my1.png" alt="">
          <p>我的活动</p>
        </li>
        <li>
          <img src="/static/my/my2.png" alt="">
          <p>我的传单</p>
        </li>
        <li>
          <img src="/static/my/my3.png" alt="">
          <p>邀请函</p>
        </li>
        <li>
          <img src="/static/my/my4.png" alt="">
          <p>帮助中心</p>
        </li>
        <li>
          <img src="/static/my/my5.png" alt="">
          <p>我的客服</p>
        </li>
        <li>
          <img src="/static/my/my6.png" alt="">
          <p>安全退出</p>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
    }
  },

  created () {
  }
}
</script>

<style>
  .headerbg{
    width: 100%;
    height: 150px;
  }
  .headerbg img{
    height: 100%;
    width: 100%;
  }
  .title{
    padding-left: 15px;
    padding-right: 15px;
    height: 120px;
  }
  .headertext{
    width: 100%;
    height: 120px;
    background:white;
    margin-top: -60px;
    border-radius: 10px;
  }
  .time {
    padding-left: 15px;
    padding-right: 15px;
    height: 80px;
  }
  .timecontent{
    width: 100%;
    height: 80px;
    background: #9FE6FF;
    margin-top: -40px;
    border-radius: 10px;
  }
  .alltime{
    width: 100%;
    height: 40px;
    position: absolute;
    bottom: 0px;
    line-height: 40px;
    letter-spacing: 2px;
  }
  .alltime span{
    vertical-align: middle;
  }
  .alltime .huiyuan{
    margin-left: 15px;
    font-size: 14px;
    color: #1179FF;
  }
  .alltime .daoqi{
    color: #000000;
    font-size: 12px;
  }
  .alltime img{
    width: 20px;
    height: 20px;
    padding-left: 15px;
    vertical-align: middle;
  }

  ul{
    width: 100%;
    display: flex;
    flex-wrap: wrap;
  }
  ul li {
    width: 25%;
    text-align: center;
    /*background: red;*/
    color: #000000;
    font-size: 12px;
    letter-spacing: 1px;
  }
  ul li img {
    height: 21px;
    width: 21px;
  }
  ul li p{
    padding-top: 8px;
    padding-bottom: 20px;
    letter-spacing: 2px;
  }
</style>

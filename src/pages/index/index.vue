<template>
  <div>
    <!--banner-->
    <div>
      <swiper :indicator-dots="swiperParams.indicatorDots"
              :autoplay="swiperParams.autoplay"
              :interval="swiperParams.interval"
              indicator-color="rgba(255, 255, 255, .5)"
              indicator-active-color="rgba(255, 255, 255, 1)"
              :duration="swiperParams.duration"
              :circular="swiperParams.circular" style="height: 220px;">
        <div>
          <swiper-item>
            <image lazy-load="true" src="/static/home/banner.png" class="slide-image">
            </image>
          </swiper-item>
        </div>
      </swiper>
    </div>

    <div class="contentlist" style="height:auto;width: 100%;background: white;border-radius: 10px;margin-top: -20px;position: absolute">
      <div class="itemtype">
        <div>
          <img src="/static/home/item1.png" alt="">
          <p>微活动</p>
        </div>
        <div>
          <img src="/static/home/item2.png" alt="">
          <p>微传单</p>
        </div>
        <div>
          <img src="/static/home/item3.png" alt="">
          <p>邀请函</p>
        </div>
      </div>

      <swiper :indicator-dots="swiperParams.indicatorDots"
              :autoplay="swiperParams.autoplay"
              :interval="swiperParams.interval"
              indicator-color="rgba(255, 255, 255, .5)"
              indicator-active-color="rgba(255, 255, 255, 1)"
              :duration="swiperParams.duration"
              :circular="swiperParams.circular" style="height: 64px;width: 100%;margin-top: 17px">
            <swiper-item>
              <div style="padding-left: 15px;padding-right: 15px;">
                <div style="width: 100%;height: 64px;">
                  <image lazy-load="true" src="/static/home/banner2.png" class="slide-image">
                  </image>
                </div>
              </div>
            </swiper-item>
            <swiper-item>
              <div style="padding-left: 15px;padding-right: 15px;">
                <div style="width: 100%;height: 64px;">
                  <image lazy-load="true" src="/static/home/banner2.png" class="slide-image">
                  </image>
                </div>
              </div>
            </swiper-item>
      </swiper>

      <!--精选模版-->
      <div style="width: 100%;height: 48px;line-height: 48px;padding-left: 15px;color: #000000;font-size: 14px;font-weight: bold;letter-spacing: 1px;">精选模板</div>
      <div class="">
        <ul>
          <li>
            <img src="/static/home/banner.png" alt="" class="bg">
            <p>999人制作</p>
            <img src="/static/home/zhizuo.png" alt="" class="zhizuo">
          </li>
          <li>
            <img src="/static/home/banner.png" alt="" class="bg">
            <p>999人制作</p>
            <img src="/static/home/zhizuo.png" alt="" class="zhizuo">
          </li>
          <li>
            <img src="/static/home/banner.png" alt="" class="bg">
            <p>999人制作</p>
            <img src="/static/home/zhizuo.png" alt="" class="zhizuo">
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  data () {
    return {
      swiperParams:　{
        indicatorDots: true,
        autoplay: true,
        interval: 1000,
        duration: 900,
        circular: true
      }
    }
  },
  methods: {
  },

  created () {
    // let app = getApp()
  }
}
</script>

<style scoped>
  .slide-image{
    height: 100%;
    width: 100%;
  }
  .itemtype{
    margin-top: 17px;
    display: flex;
  }
  .itemtype div{
    flex: 1;
    text-align: center;
    font-size: 14px;
    color: #000000;
    letter-spacing: 2px;
  }
  .itemtype div p{
    padding-top: 8px;
  }
  .itemtype div img{
    height: 44px;
    width: 44px;
  }
  ul{
    width: 100%;
    display: flex;
    flex-wrap: wrap;
  }
  ul li {
    width: 33.3%;
    height: 184px;
    position: relative;
    /*background: red;*/
    color: #000000;
    font-size: 12px;
    letter-spacing: 1px;
  }
  ul li p {
    position: absolute;
    /*left: 0px;*/
    bottom: 11px;
    left: 7%;
  }
  ul li img.bg{
    height: 150px;
    width: 86%;
    position: absolute;
    left: 50%;
    margin-left: -43%;
  }
  ul li img.zhizuo{
    position: absolute;
    height: 34px;
    width: 61px;
    right: 0px!important;
    bottom: 0px;
  }
</style>

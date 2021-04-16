<template>
 <div>
   <!-- 轮播图 -->
  <div class="carousel">  
     <view> <Swiper :images="images"  /> </view>
 </div> 
 <!-- 主体 -->
  <view class="case">  
     <view class="wrapper">
    <view class="item">
      <navigator url="/pages/node/node" hover-class="navigator-hover">
        <image  src="https://img-blog.csdnimg.cn/20210415102833122.gif#pic_center"></image>
        <label class="text">通知通告</label> 
      </navigator>
    </view> 

    <view class="item">
        <navigator url="/pages/newss/newss" hover-class="navigator-hover">
          <image  src="https://img-blog.csdnimg.cn/202104151028325.gif#pic_center"></image>
          <label class="text">校园新闻</label> 
        </navigator>
      </view>
  
    <view class="item">
        <navigator url="/pages/club/club" hover-class="navigator-hover">
          <image  src="https://img-blog.csdnimg.cn/20210415102833619.gif#pic_center"></image>
          <label class="text">社联活动</label> 
        </navigator>
    </view>
   
    <view class="item">
        <navigator url="/pages/bussiness/one" hover-class="navigator-hover">
          <image  src="https://img-blog.csdnimg.cn/20210415102833705.gif#pic_center"></image>
          <label class="text">社联风采</label> 
        </navigator>
    </view>
  
    <view class="item">
        <navigator url="/pages/studyhome/studyhome" hover-class="navigator-hover">
          <image  src="https://img-blog.csdnimg.cn/20210415102832824.gif#pic_center"></image>
          <label class="text">社团申请</label> 
        </navigator>
    </view>
   
    <view class="item">
        <navigator url="/pages/studyhome/studyhome" hover-class="navigator-hover">
          <image  src="https://img-blog.csdnimg.cn/20210415102832662.gif#pic_center"></image>
          <label class="text">精彩瞬间</label> 
        </navigator>
    </view>

    <view class="item">
        <navigator url="/pages/club/main" hover-class="navigator-hover">
          <image  src="https://img-blog.csdnimg.cn/20210415102832405.gif#pic_center"></image>
          <label class="text">组织机构</label> 
        </navigator>
    </view>
   
    <view class="item">
        <navigator url="/pages/car/car" hover-class="navigator-hover">
          <image  src="https://img-blog.csdnimg.cn/2021041510283276.gif#pic_center"></image>
          <label class="text">光荣榜</label> 
        </navigator>
    </view>
  </view>
   </view> 
   </div> 
</template>

<script>
import Swiper from '@/components/swiper'

export default {
  components: { Swiper },
  data() {
    return {
      images: [
        {
          url:
            'https://www.zut.edu.cn/_mediafile/index/2017/10/12/_thumb/3u5ed2vljk.jpg'
        },
        {
          url:
            'https://www.zut.edu.cn/_mediafile/index/2017/10/12/_thumb/3zqr3sclhg.jpg'
        },
        {
          url:
            'https://img-blog.csdnimg.cn/20210415102833988.JPG?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L205ODA4Mjg=,size_16,color_FFFFFF,t_70#pic_center'
        }
      ]
    }
  },
  methods: {},
  computed: {}
}
</script>

<style scoped>
/* .message {
  color: red;
  padding: 10px;
  text-align: center;
} */
.carousel{
	width: 100%;
	height: 400rpx;
}
image{
	width:850rpx;
}
.case-ban{
  height: 100%;
  overflow: hidden;
}
.case{
  padding:6px 8px;
  /*border:1px solid #3915db;
  background:rgba(119, 238, 115, 0.89);*/
  position: absolute;
  
}

.wrapper{
  background:rgba(220, 242, 245, 0.89);
	display:flex;
	padding:0 0px;
	flex-wrap:wrap;
  border-radius: 10px;/*圆角设置*/
}
.item{
	font-size:14px;
	box-sizing:border-box;
	height:342rpx;
  /*border:1px solid #3915db;*/
	flex:auto;
	display:flex;
	justify-content:center;
	align-items:center;
  width: 25%;
  text-align: center;
}
.item image {
  /*width: 230rpx;
  height: 230rpx;
  margin: 0 auto;
  margin-top: 0rpx;
  border-radius: 0%;*/
  width: 200rpx;
  height: 200rpx;
  margin: 0 auto;
  margin-top: 0rpx;
  border-radius: 0%;
}
.item label {
  text-align: center;
  display: block;
  line-height: 65.52rpx;
  font-size: 35rpx;
  color: rgb(62, 15, 233);
}
.item nav {
  display: block;
  line-height: 65.52rpx;
  font-size: 28.08rpx;
}
</style>
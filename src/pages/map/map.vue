<template>
	<view>
<GaodeHeader class="noDaohang" bindchangeType="changeGaodeType" type="{{gaode_type}}" NavigationOrNot="{{daohang}}"></GaodeHeader>
<view class="section">
  <!-- 当前位置 -->
  <GaodeInputTips bindcustomEvent="handleCustomEvent" city="{{city}}" longitude="{{longitude}}" latitude="{{latitude}}" defaultValue="{{'当前位置'}}" inputType="start"></GaodeInputTips>
  <!-- 目的地 -->
  <GaodeInputTips bindcustomEvent="handleCustomEvent" city="{{city_e}}" longitude="{{longitude_e}}" latitude="{{latitude_e}}" defaultValue="{{'目的地'}}" inputType="end"></GaodeInputTips>
</view>
<view class="map_container">
  <map wx:if="{{gaode_type !== 'bus' && mapState}}" class="map" id="map" longitude="{{longitude}}" latitude="{{latitude}}" scale="14" show-location="true" markers="{{markers}}" bindmarkertap="makertap" polyline="{{polyline}}" include-points="{{includePoints}}"></map>
  <!-- 公交 -->
  <view wx:if="{{gaode_type === 'bus' && mapState}}">
    <view class="text_box" wx:for="{{transits}}" wx:for-item="i" wx:key="i">
      <text class="text_item" wx:for="{{i.transport}}" wx:for-item="j" wx:key="j">
        {{j}}
      </text>
    </view>
  </view>
  <!-- 搜索错误 -->
  <view wx:if="{{!mapState}}">搜索中...</view>
</view>
<view class="map_text">
  <text class="h1">{{textData.name}}</text>
  <text>{{textData.desc}}</text>
  <view class="text_box" wx:if="{{daohang}}">
    <view class="text">{{distance}}</view>
    <view class="text">{{cost}}</view>
  </view>
</view>

		<button class="changemp">切换至热力图</button>
	    <view class="sub-nav">
	        <navigator url="../index/index" class="sn1">首页</navigator>
	        <navigator url="#" class="sn2">地图</navigator>    
	        <navigator url="../ana_images/ana_images" class="sn3">上传</navigator>
	        <navigator url="../wode/wode" class="sn4">我的</navigator>
	    </view>
	</view>
</template>

<script>
	import "../../static/css/normalize.css";
	import "../../static/css/map.css";
	import "../../static/js/map.js";

	export default {

	  
	};
</script>



<style scoped>
@font-face {
    font-family: 'icomoon';
    src:  url('../../static/fonts/icomoon.eot?e068fy');
    src:  url('../../static/fonts/icomoon.eot?e068fy#iefix') format('embedded-opentype'),
      url('../../static/fonts/icomoon.ttf?e068fy') format('truetype'),
      url('../../static/fonts/icomoon.woff?e068fy') format('woff'),
      url('../../static/fonts/icomoon.svg?e068fy#icomoon') format('svg');
    font-weight: normal;
    font-style: normal;
    font-display: block;
}

.section{
  height: 80px;
  width: 100%;
}
.section input{
  width:90%;
  margin:5px auto;
  border:1px solid #c3c3c3;
  height:30px;
  border-radius: 3px;
  padding: 0 5px;
}
.map_container{
  position: absolute;
  top: 115px;
  bottom: 80px;
  left: 0;
  right: 0;
}
.map{
  width: 100%;
  height: 100%;
}
.map_text{
  position: absolute;
  left: 0;
  right: 0;
  bottom: 0px;
  height: 80px;
  background: #fff;
  padding: 0 15px;
}
text{
  margin: 5px 0;
  display: block;
  font-size:12px;
}
.h1{
  margin: 15px 0;
  font-size:15px;
}
/* 公交样式 */
.text_box{
  margin: 0 15px;
  padding: 15px 0;
  border-bottom: 1px solid #c3c3c3;
  font-size: 13px;
}
.text_box .text_item{display:inline-block;line-height: 8px;}
</style>

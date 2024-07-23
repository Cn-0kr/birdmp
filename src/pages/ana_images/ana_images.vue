<template>
	<view>
		  <view class="ana_bg">
		    <view class="abg1"></view>
		    <view class="abg2"></view>
		    <view class="abg3"></view>
		    <button class="upload">
		      <view class="yyy">
		        <view class="track"></view>
		        <view class="texxxt">点击上传图片</view>
		      </view>
		    </button>
		  </view>
		
	    <view class="sub-nav">
	        <navigator url="../index/index" class="sn1">首页</navigator>
	        <navigator url="../map/map" class="sn2">地图</navigator>    
	        <navigator url="#" class="sn3">上传</navigator>
	        <navigator url="../wode/wode" class="sn4">我的</navigator>
	    </view>
	</view>
</template>

<script>
	import "../../static/css/normalize.css";
	import "../../static/css/ana_images.css";
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			
		}
	}
</script>

<style>
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
</style>

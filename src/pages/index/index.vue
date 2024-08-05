<template>
	<view>
		
	    <view class="top-nav">
	        <navigator url="#" class="ranking">鸟类排行榜</navigator>
	        <view class="searchbar"></view>
	        <navigator url="#" class="noobintro">新手引导</navigator>
	    </view>
	    
	    
		<view class="lists">
			<view class="item" v-for="(item,index) in 15" :key="index">
				{{index+1}}
			</view>
		</view>
	
	    <view class="sub-nav">
	        <navigator url="#" class="sn1">首页</navigator>
	        <navigator url="../map/map" class="sn2">地图</navigator>    
	        <navigator url="../ana_images/ana_images" class="sn3">上传</navigator>
	        <navigator url="../wode/wode" class="sn4">我的</navigator>
	    </view>
	</view>
</template>

<script>
	import "../../static/css/normalize.css";
	import "../../static/css/index.css";


	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
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
  .lists{
    padding: 20rpx;
    box-sizing: border-box;
    column-count: 2;
    column-gap: 10rpx;
  }
  
  .item{
    break-inside: avoid;
    width: auto;
    height: 200rpx;
    background-color: #eee;
    line-height: 200rpx;
    text-align: center;
    margin-bottom: 10rpx;
  }
  
  .lists .item:nth-child(2n+1){
    height: 240rpx;
  }
  .lists .item:nth-child(3n+1){
    height: 320rpx;
  }
</style>
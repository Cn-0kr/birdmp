<template>
	<view>
		<view class="map-container">
			<image class="map" src="../../static/images/map.png" mode="widthFix"></image>
			<button class="changemp">切换至热力图</button>
		</view>
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

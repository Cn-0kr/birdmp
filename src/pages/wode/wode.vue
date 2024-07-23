<template>
	<view>
		<view class="header">
		  <navigator url="#" class="icon"></navigator>
		  <navigator url="#" class="username">用户名</navigator>
		</view>
		<view class="wode-nav">
		  <!-- 浏览历史 我的发布 已发现鸟类 观鸟记录 -->
		  <view class="wn1">关于帖子</view>
		  <view class="local-nav">
		    <view class="local-nav-item">
		      <navigator url="#" title="浏览历史">
		        <text class="local-nav-icon"></text>
		        <text>浏览历史</text>
		      </navigator>
		    </view>
		    <view class="local-nav-item">
		      <navigator url="#" title="我的发布">
		        <text class="local-nav-icon"></text>
		        <text>我的发布</text>
		      </navigator>
		    </view>
		  </view>
		  <view class="wn2">关于观鸟</view>
		  <view class="local-nav1">
		    <view class="local-nav1-item">
		      <navigator url="#" title="已发现鸟类">
		        <text class="local-nav1-icon"></text>
		        <text>已发现鸟类</text>
		      </navigator>
		    </view>
		    <view class="local-nav1-item">
		      <navigator url="#" title="观鸟记录">
		        <text class="local-nav1-icon"></text>
		        <text>观鸟记录</text>
		      </navigator>
		    </view>
		  </view>
		  <view class="wn3">联系我们</view>
		
		  <button class="logout">
		      <text class="texxxt">退出登录</text>
		  </button>
		</view>
		
	    <view class="sub-nav">
	        <navigator url="../index/index" class="sn1">首页</navigator>
	        <navigator url="../map/map" class="sn2">地图</navigator>    
	        <navigator url="../ana_images/ana_images" class="sn3">上传</navigator>
	        <navigator url="#" class="sn4">我的</navigator>
	    </view>
	</view>
</template>


<script>
	import "../../static/css/normalize.css";
	import "../../static/css/wode.css";
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

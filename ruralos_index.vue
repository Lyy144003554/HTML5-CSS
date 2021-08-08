<template>
	<view class="content">
		<image class="logo" src="/static/ruralos.png"></image>
		<view class="text-area">
			<text class="title1">{{title1}}</text>
		</view>
		<view class="button1" onclick="tiaozhuan">
		<button type="primary" plain="true">进入</button>
		</view>
		<view class="button2">
		<button type="primary" plain="true">关于</button>
		</view>
		<view class="button3">
		<button type="warn" plain="true">退出</button>
		</view>
		<view class="text">
			<text class="title2">{{title2}}</text>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title1: 'RuralOS·重新定义未来农村',
			    title2:'版本号-2021.02.21',
				
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
	function tiaozhuan()
	{
		
	}
</script>

<style>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}
	
	.button1{
		height: 200rpx;
		width: 400rpx;
		margin-left: auto;
		margin-right: auto;
		margin-top: 50rpx;
		
	}
	
	.button2{
		height: 200rpx;
		width: 400rpx;
		margin-left: auto;
		margin-right: auto;
		margin-top: -70rpx;
	}
	.button3{
		height: 200rpx;
		width: 400rpx;
		margin-left: auto;
		margin-right: auto;
		margin-top: -70rpx;
	}

	.logo {
		height: 200rpx;
		width: 600rpx;
		margin-top: 200rpx;
		justify-content: center;
		margin-bottom: 50rpx;
	}

	.text-area {
		display: flex;
		justify-content: center;
		font-size: 45rpx;
		font-weight:bold;
		
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
	.text{
		color: #8F8F94;
		margin-top: 130rpx;
		font-size: smaller;
	}
</style>

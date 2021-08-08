<template>
	<view>
		<cu-custom bgColor="bg-gradual-red" :isBack="true">
			<block slot="content">阳光房屋</block>
			<block slot="backText">返回</block>
			</cu-custom>
				<view class="content1">
					<image class="logo" src="/static/ljt.jpg"></image>
					<view class="text-area">
					<text class="title1">智能分类垃圾桶1.0</text>
					</view>
					<view class="button1">
					<button>查看详情</button>
					</view>
				</view>
				<view class="content2">
					<image class="logo" src="/static/ljt2.jpg"></image>
					<view class="text-area">
					<text class="title1">智能分类垃圾桶2.0</text>
					</view>
					<view class="button1">
					<button>查看详情</button>
					</view>
				</view>
				<view class="cu-bar tabbar bg-white shadow foot">
					<view class="action" @click="NavChange" data-cur="basics">
						<view class='cuIcon-cu-image'>
							<image :src="'/static/tabbar/basics' + [PageCur=='basics'?'_cur':''] + '.png'"></image>
						</view>
						<view :class="PageCur=='basics'?'text-green':'text-gray'">阳光房屋</view>
					</view>
					<view class="action" @click="NavChange" data-cur="component">
						<view class='cuIcon-cu-image'>
							<image :src="'/static/tabbar/component' + [PageCur == 'component'?'_cur':''] + '.png'"></image>
						</view>
						<view :class="PageCur=='component'?'text-green':'text-gray'">设计采购</view>
					</view>
					<view class="action" @click="NavChange" data-cur="plugin">
						<view class='cuIcon-cu-image'>
							<image :src="'/static/tabbar/plugin' + [PageCur == 'plugin'?'_cur':''] + '.png'"></image>
						</view>
						<view :class="PageCur=='plugin'?'text-green':'text-gray'">循环检测</view>
					</view>
					<view class="action" @click="NavChange" data-cur="component">
						<view class='cuIcon-cu-image'>
							<image :src="'/static/tabbar/component' + [PageCur == 'component'?'_cur':''] + '.png'"></image>
						</view>
						<view :class="PageCur=='component'?'text-green':'text-gray'">交流社区</view>
					</view>
				</view>
			</view>
		</template>
		
		<script>
			export default {
				data() {
				return {
						PageCur: 'basics'
					}
				},
				methods: {
					NavChange: function(e) {
						this.PageCur = e.currentTarget.dataset.cur
					}
				}
			}
		</script>
		
		<style>
				
			.content1{
				height: 350rpx;
				width: 300rpx;
				display: flex;
				flex-direction: column;
				margin-left:50rpx;
				margin-right: auto;
				margin-top: 70rpx;
		        font-size: 35rpx;
			}
			.content2{
				height: 350rpx;
				width: 300rpx;
				display: flex;
				flex-direction: column;
				margin-left:400rpx;
				margin-right: auto;
				margin-top: -350rpx;
			    font-size: 35rpx;
			}
		
		</style>

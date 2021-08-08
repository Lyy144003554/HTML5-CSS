<template>
	<view>
		<cu-custom bgColor="bg-gradual-red" :isBack="true"><block slot="backText">返回</block>
		<block slot="content">我的晾衣架</block></cu-custom>
		<view class="cu-timeline">
			<view class="cu-time">昨天</view>
			<view class="cu-item">
				<view class="content">
					<text>22:30</text> 
				</view>
			</view>
			<view class="cu-item">
				<view class="content">
					<text>21:32</text> 衣物干湿程度预计完成75%。
				</view>
			</view>
			<view class="cu-item">
				<view class="content">
					<text>20:30</text> 第x次调整到合适距离。
				</view>
			</view>
			<view class="cu-item">
				<view class="content">
					<text>20:00</text> 检测到衣物开始悬挂。
				</view>
			</view>
		</view>
		<view class="cu-timeline">
			<view class="cu-time">02-21</view>
			<view class="cu-item">
				<view class="content">
					<text>02:30</text> 衣物干湿程度预计完成95%。
				</view>
			</view>
			<view class="cu-item">
				<view class="content">
					<text>01:28</text> 第x次调整到合适距离。
				</view>
			</view>
			<view class="cu-item">
				<view class="content">
					<text>00:37</text> 检测到衣物开始悬挂。
				</view>
			</view>
		</view>
		</view>
</template>

<script>
	export default {
		data() {
			return {

			};
		}
	}
</script>
<style>
</style>

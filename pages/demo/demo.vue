<template>
	<view>
		<view class="view-box animated" hover-stay-time="800" hover-class="view-box-hover rubberBand">第一个box</view>
		<text :selectable="true">这是text \n 这是text \n  这是text \n</text>
		<view class="view-box" id="view2">第一个box</view>
	</view>
</template>

<script>
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
.view-box{
	width: 200upx;
	height: 200upx;
	background: #007AFF;
	color: #FFFFFF;
	margin: 100upx;
}
.view-box-hover{
	background: red;
}
#view2{
	background: yellow;
	color: black;
}
</style>

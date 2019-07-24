<template>
	<view>
		<!-- <view class="view-box animated" hover-stay-time="800" hover-class="view-box-hover rubberBand">第一个box</view>
		<text :selectable="true">这是text \n 这是text \n  这是text \n</text>
		<view class="view-box" id="view2">第一个box</view> -->
		<view class="box">
			<text>text组件</text>
			<view>1</view>
			<view>2</view>
			<view>3</view>
			<view>4</view>
		</view>
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
.box{
	width: 300upx;
	height: 300upx;
	background: #007AFF;
	color: #FFFFFF;
	margin: 100upx;
	padding: 50upx;
}
.box view{
	font-size: 40upx;
}
/* .box>view:nth-of-type(1){
	background: #09BB07;
}
.box>view:nth-of-type(2){
	background: red;
}
.box>view:nth-of-type(3){
	background: pink;
} */
/* .box>view:first-child{
	background: red;
}
.box>view:last-child{
	background: pink;
} */

/* .box>view:first-of-type{
	background: red;
}
.box>view:last-of-type{
	background: pink;
} */
/* .box>view:nth-of-type(2n-1){
	background: red;
}
.box>view:nth-of-type(2n){
	background: pink;
} */
.box>view:nth-of-type(even){
	background: red;
}
.box>view:nth-of-type(odd){
	background: pink;
}
</style>

<template>
	<view>
		<view :class="classname">
			<view>{{username}}</view>
			<view>{{userinfo.username}}</view>
			<!-- <view>{{itemdata}}</view> -->
		</view>
		<button type="default" @tap="changeUsername('Alex')">修改名字</button>
		<button type="default" @tap="changeClassname('box2')">修改</button>
		
	</view>

</template>

<script>
	export default {
		data() {
			return {
				username: "Tom",
				userinfo:{
					username:"Jack"
				},
				classname: "box"
			}
		},
		methods:{
			changeUsername:function(name){
				this.userinfo.username = "aaa"+name
			},
			changeClassname:function(newclass){
				this.classname = newclass
			}
		}
	}
</script>

<style>
.box{
	border: 1upx solid #333333;
	height: 500upx;
	width: 100%;
	display: flex;
}
.box2{
	border: 1upx solid #1AAD19;
	height: 500upx;
	width: 100%;
	display: flex;
}
.box>view{
	background: #007AFF;
	color: white;
	font-weight: bold;
	font-size: 35upx;
	display: flex;
	flex: 1;
	height: 500upx;
	justify-content: center;
	align-items: center;
	border: 1upx solid #FFFFFF;
}
.box2>view{
	background: #09BB07;
	color: white;
	font-weight: bold;
	font-size: 35upx;
	display: flex;
	flex: 1;
	height: 500upx;
	justify-content: center;
	align-items: center;
	border: 1upx solid #FFFFFF;
}
</style>

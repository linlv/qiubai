<template>
	<view>
		<!-- <view>{{name}}</view> -->
		<view>{{num}}</view>
		<view>{{num>10?'Yes':'No'}}</view>
		<button type="primary" @tap="change()">修改</button>
	</view>
</template>

<script>
	export default{
		data(){
			return{
				name:"我是一个名称",
				num:0
			}
		},
		watch:{
			name:function(val){
				console.log(val)
			},
			num:function(val){
				console.log(val)
			}
		},
		methods:{
			change:function(){
				// this.name="被修改"
				this.num++
			}
		}
	}
</script>

<style>

</style>
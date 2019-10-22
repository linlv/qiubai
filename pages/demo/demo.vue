<template>
	<view>
		
		<view>
			{{Transweight}}
		</view>
		
	</view>
</template>

<script>
	export default{
		data(){
			return{
				//体重
				weight:1900
			}
		},
		computed:{
			Transweight:function(){
				return this.weight>1000 ? (this.weight/1000)+'kg' : this.weight+'g'
			}
		},
		methods:{
			
		}
	}
</script>

<style>

</style>
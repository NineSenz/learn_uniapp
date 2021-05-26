<template>
	<view>
		<button @click="sendGet">发送请求</button>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			sendGet(){
				uni.request({
					url: 'localhost:8080/home/swiper',
					success(res){
						console.log(res)
					}
				})
			}
		}
	}
</script>

<style>

</style>

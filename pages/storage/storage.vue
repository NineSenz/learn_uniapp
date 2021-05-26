<template>
	<view>
		<button @click="setStorage">存储数据</button>
		<button @click="getStorage">获取数据</button>
		<button @click="removeId">删除数据</button>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			setStorage(){
				uni.setStorage({
					key:'id',
					data: 80,
					success() {
						console.log('存储成功')
					}
				})
			},
			
			getStorage(){
				uni.getStorage({
					key:'id',
					success(res){
						console.log('获取成功', res)
					}
				})
			},
			
			removeId(){
				uni.removeStorage({
					key:'id',
					success(){
						console.log('删除成功')
					}
				})
			}
		}
	}
</script>

<style>

</style>

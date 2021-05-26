<template>
	<view>
		<button @click="chooseImg">上传图片</button>
		<image v-for="item in imgArr" :src="item" @click="previewImg(item)"></image>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				imgArr: []
			}
		},
		methods: {
			chooseImg(){
				console.log('上传图片')
				uni.chooseImage({
					count:5,
					success:res => {   // this指向问题，用箭头函数可以解决
						this.imgArr = res.tempFilePaths
						console.log(this.imgArr)
					}
				})
			},
			previewImg(current){
				uni.previewImage({
					current:current,
					urls: this.imgArr,
					loop: true,
					indicator: 'number'
				})
			}
		}
	}
</script>

<style>

</style>

<template>
	<view>
	        <h1>{{ title }}</h1>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {
			console.log("页面加载了")
		},
		onShow() {
			console.log("页面显示了")
		},
		onHide() {
			console.log("页面隐藏了")
		},
		onReady() {
			console.log("页面初次渲染完成")
		},
		methods: {

		}
	}
</script>

<style>
	
</style>

<template>
	<view>
		<view>{{ title }}</view>
		<view>{{ 1+1 }}</view>
		<view>{{ flag?'返回为真':'返回为假' }}</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: "数据绑定",
				flag: true
			}
		},
		methods: {
			
		}
	}
</script>

<style>

</style>

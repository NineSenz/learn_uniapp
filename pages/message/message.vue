<template>
	<view>
		<view>{{ title }}</view>
		<view>{{ 1+1 }}</view>
		<view>{{ flag?'返回为真':'返回为假' }}</view>
		<image v-bind:src="imgUrl"></image>
		<view v-for="(item, index) in hero" :key="item.id">
			序号: {{ item.id }},名字:{{ item.name }}, 年龄: {{ item.age }}
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: "数据绑定",
				flag: true,
				imgUrl:"/static/img/1.JPG",
				hero: [
					{
						id: 1,
						name: "瑞雯",
						age: 18
					},
					{
						id: 2,
						name: "德玛西亚",
						age: 21
					},
					{
						id: 3,
						name: "男爵",
						age: 32
					}
				]
			}
		},
		methods: {
			
		}
	}
</script>

<style>

</style>

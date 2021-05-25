<template>
	<view>
		<view >
			<ul v-for="item in list">
				<li>{{item}}</li>
			</ul>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				msg: "hello",
				list: ['frontend','backend', 'database','testcase', 'application']
			}
		},
		onPullDownRefresh(){
			setTimeout(()=>{
				this.list = ['testcase', 'application','frontend','backend', 'database']
				uni.stopPullDownRefresh()
			},2000)
		},
		methods: {
			
		}
	}
</script>

<style>

</style>

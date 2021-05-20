<template>
	<view>
		<view class="box" hover-class="box-active">
			<view class="box2" hover-class="box2-active" hover-stop-propagation>小盒子</view>
		</view>
		<view>
			<p>
				<b>hover-stop-propagation</b>属性可以解决事件冒泡的问题
			</p>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			
		}
	}
</script>

<style>
	.box {
		width: 200px;
		height: 200px;
		background: #007AFF;
	}
	.box-active {
		background: red;
	}
	.box2 {
		width: 100px;
		height: 100px;
		background: #4CD964;
	}
	.box2-active {
		background: #F0AD4E;
	}
</style>

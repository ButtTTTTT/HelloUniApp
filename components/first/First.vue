<template>
	<view>
		<button @click="buttonClick">{{title}}</button>
	</view>
</template>

<script>
	export default{
		data(){
			return{
				title:"点我",
			}
		},
		onLoad(){
			//页面启动的生命周期，这里编写页面加载时的逻辑
		},
		//多个页面生命周期监听，在这里继续写。逗号分隔
		methods: {
			buttonClick(){
				this.title = "我被脏东西碰了"
			},
		}
	}
	
</script>

<style>
	button{
		background-color: red;
	}
</style>
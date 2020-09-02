<template>
	<div>
		<div class="title">热门推荐</div>
		<div class="menu">
			<ul>
				<li @click="menu1">笔记本</li>
				<li @click="menu2">手机</li>
				<li>服饰</li>
				<li>手表</li>
				<li>书籍</li>
				<li>玩具</li>
				<li>家电</li>
				<li>学习用品</li>
				<li>洗漱用品</li>
				<li>宠物用品</li>
			</ul>
		</div>
	</div>
</template>

<script>
	import Msg from './Msg.js'
	export default{
		methods:{
			menu1:function(){
				Msg.$emit("val","1");
			},
			menu2:function(){
				Msg.$emit("val","2");
			}
		}
	}
</script>

<style>
	.title{
		width: 100px;
		color: red;
	}
	.menu li{
		list-style: none;
		height: 50px;
		margin-bottom: 2px;
		background-color: white;
		line-height: 50px;
		cursor: pointer;
	}
</style>

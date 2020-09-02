<template>
	<div class="main">
		<div class="left">
			<Left></Left>
		</div>
		<div class="right">
			<div class="top">
				<img src="../../public/img/title.png" />
			</div>
			<div class="buttom">
				<Right></Right>
			</div>
		</div>
		
	</div>
</template>

<script>
 import Right from '../components/Right.vue'
 import Left from '../components/Left.vue'
	export default{
		components:{
			Left,
			Right
		}
	} 
</script>

<style type="text/css">
	*{
		padding: 0;
		margin: 0;
	}
	.left{
		width: 100px;
		float: left;
		margin-right: 10px;
	}
	.right{
		width: 1000px;
		float: left;
		margin-left: 10px;
 	}
	.main{
		width: 1200px;
		margin: 20px auto;
	}
	.top img{
		width: 1000px;
		height: 200px;
	}
	.left,.right{
		background-color: #f5f5f5;
		height: 500px;
	}
	.buttom{
		
	}
</style>

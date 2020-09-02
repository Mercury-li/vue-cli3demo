<template>
	<div>
		<div v-if="test==1">
			<GoodList :goodId="1"></GoodList>
		</div>
		<div v-else-if="test==2">
			<GoodList :goodId="2"></GoodList>
		</div>
		<div v-else>
			<GoodList :goodId="0"></GoodList>
		</div>
	</div>
</template>

<script>
	import Msg from './Msg.js'
	import GoodList from './GoodList.vue'
	export default {
		data() {
			return {
				test: 0
			}
		},
		mounted: function() {
			var _this = this;
			Msg.$on('val', function(m) {
				_this.test = m;
			})
		},
		components: {
			GoodList
		}
	}
</script>

<style>
</style>

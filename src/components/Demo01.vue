<template>
	<div>
		<h1 id="demo">{{name}}</h1>
		<button @click="info()">点我显示</button>
	</div>
</template>

<script>
	export default {
		name:'Demo01',
		data() {
			return {
				name: 'zhangsan',
				age:18,
				
			}
		},
		computed:{
			show(){
				
				return this.name + '今年' + this.age
			}
		},
		methods:{
			info(){
				alert(this.show)
			}
		}
	}
</script>

<style>
	#demo{
		font-size: 40px;
		background-color: aquamarine;
	}
</style>
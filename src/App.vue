<!--
 * @LastEditTime: 2019-11-27 11:48:12
 * @Description: 
 * @Date: 2019-11-27 11:44:55
 * @Author: @虾哔哔
 -->
<template>
	<div id="app">
		<Test1 />
	</div>
</template>

<script>
	import Test1 from "./components/test1";
	export default {
		name: "app",
		components: {
			Test1
		}
	};
</script>

<style lang="less">
	#app {
		font-family: "Avenir", Helvetica, Arial, sans-serif;
		-webkit-font-smoothing: antialiased;
		-moz-osx-font-smoothing: grayscale;
		color: #2c3e50;
	}
</style>

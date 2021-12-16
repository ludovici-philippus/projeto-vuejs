<template>
	<Header/>
	<Main/>
	<Footer/>
</template>

<script>
	import Header from "./components/header.vue";
	import Main from "./components/main.vue";
	import Footer from "./components/footer.vue";

	export default{
		name: "App",
		components:{
			Header,
			Main,
			Footer,
		}
	}
</script>

<style>
	*{
		margin: 0;
		padding: 0;
		box-sizing: border-box;
	}

	html, body{
		height: 100%;
	}

	.container{
		max-width: 1280px;
		margin: auto;
		padding: 0 2%;
	}

	.w33{
		width: 33.3%;
	}

	.w50{
		width: 50%;
	}

	.w100{
		width: 100%;
	}
</style>

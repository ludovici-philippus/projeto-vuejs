<template>
	<footer>
		<p>{{ texto  }}</p>
	</footer>
</template>

<script>
	export default{
		name: "Footer",
		data(){
			return{
				texto: "Propriedade intelectual é meu ovo",
			}
		}
	}
</script>

<style scoped>
	footer{
		background-color: steelblue;
		padding: 5px 0;
		text-align: center;
		color: white;
	}
</style>

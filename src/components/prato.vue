<template>
	<div class="prato-single">
		<div class="prato-head">
			<img :src="imagem">
		</div>		
		<div class="prato-body">
			<h3>{{ nome_prato  }}</h3>
			<p>{{ descricao_prato }}</p>
		</div>
	</div>
</template>

<script>
	export default{
		name: "Prato",
		data(){
			return{

			}
		},
		props:{
			"imagem": String,
			"nome_prato": String,
			"descricao_prato": String,
		}
	}
</script>

<style scoped>
	.prato-single{
		display: flex;
		flex-direction: column;
		align-content: flex-end;
		align-items: center;
	}

	.prato-head{
		max-width: 300px;
	}
	.prato-head img{
		width: 100%;
	}
</style>

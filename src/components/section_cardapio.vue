<template>
	<section class="cardapio">
		<div class="container">
			<h2>Cardápio</h2>
			<div class="pratos">
				<Prato :imagem="prato_1.imagem" :nome_prato="prato_1.nome" :descricao_prato="prato_1.descricao" />
				<Prato :imagem="prato_2.imagem" :nome_prato="prato_2.nome" :descricao_prato="prato_2.descricao" />
				<Prato :imagem="prato_3.imagem" :nome_prato="prato_3.nome" :descricao_prato="prato_3.descricao" />	
			</div>
		</div>	
	</section>
</template>

<script>
	import Prato from "./prato.vue";
	export default{
		name: "Cardapio",
		data(){
			return{
				prato_1: {
					imagem: "./img/sushi1.jpeg",
					nome: "Sushi 1",
					descricao: "Lorem Ipsum idom eu não sei mais o que kkj",
				},
				prato_2: {
					imagem: "./img/sushi2.jpg",
					nome: "Sushi 2",
					descricao: "Lorem Ipsum idom eu não sei mais o que kkj",
				},
				prato_3: {
					imagem: "./img/sushi3.jpg",
					nome: "Sushi 3",
					descricao: "Lorem Ipsum idom eu não sei mais o que kkj 3",
				}
			}
		},
		components:{
			Prato,
		}
	}
</script>

<style scoped>
	.pratos{
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		align-items: center;
	}	
</style>

<template>
	<main>
		<ImageApresentacao/>
		<Cardapio/>
		<SobreNos/>
	</main>
</template>

<script>
	import ImageApresentacao from "./image_apresentacao.vue";
	import Cardapio from "./section_cardapio.vue";
	import SobreNos from "./section_sobre_nos.vue";
	export default{
		name: "Main",
		data(){
			return{

			}
		},
		components:{
			ImageApresentacao,
			Cardapio,
			SobreNos,
		}
	}
</script>

<style scoped>
	.image-bg{
		margin-bottom: 20px;
	}

	.cardapio{
		margin-bottom: 20px;
	}
	.sobre-nos{
		margin-bottom: 20px;
	}

</style>

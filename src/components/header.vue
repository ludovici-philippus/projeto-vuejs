<template>
	<header>
		<div class="container">
			<div class="logo">
				<h1>{{ company  }}</h1>
			</div>
			<div class="menu">
				<ul>
					<li><a :href="link.home">Home</a></li>
					<li><a @click="sobre" :href="link.sobre">Sobre</a></li>
					<li><a @click="contato" :href="link.contato">Contato</a></li>
				</ul>
			</div>
		</div>	
	</header>
</template>

<script>
	export default{
		name: "Header",
		data(){
			return{
				company: "Hamburgueria",
				link: {
					home: "http://localhost:8080/",
					sobre: "http://localhost:8080/#sobre",
					contato: "http://localhost:8080/#contato",
				},
			}
		},
		methods:{
			sobre(){
				alert("Clicou em Sobre!");
			},
			contato(){
				alert("Clicou em Contato!");
			}
		}
	}
</script>

<style scoped>
	header{
		background-color: steelblue;
		color: white;
		padding: 10px 0;
	}

	header .container{
		display: flex;
		flex-direction: row;
		justify-content: space-between;
	}
	
	ul{
		list-style: none;
	}

	li{
		display: inline-block;
		margin-right: 8px;
		margin-top: 8px;
	}

	li a{
		text-decoration: none;
		color: white;
		transition: 0.5s;
	}

	li a:hover{
		color: indianred
	}
</style>

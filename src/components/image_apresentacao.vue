<template>
	<div class="image-bg">
		<div class="overlay">
			<div class="content">
				<h2>Hamburgueria seu jorge</h2>
				<p>A melhor da região!</p>
			</div>
		</div>
	</div>
</template>

<script>
	export default{
		name: "ImageApresentacao",
		data(){
			return{
	
			}
		}
	}
</script>

<style scoped>
	.image-bg{
		background-image: url("../../public/img/bg-form.jpg");
		background-repeat: no-repeat;
		background-size: cover;
		background-position: center;
		width: 100%;
		min-height: 30vh;
	}
	
	.overlay{
		background-color: rgba(0, 0, 0, 0.5);
		width: 100%;
		min-height: 30vh;
		position: relative;
		top: 0;
		left: 0;
	}

	.content{
		position: absolute;
		top: 50%;
		left: 50%;
		color: white;	
		transform: translate(-50%, -50%);
		text-align: center;
	}

	.content h2{
		font-size: 24px;
	}

	.content p{
		font-size: 16px;
	}

</style>

<template>
	<div class="row hero">
		<div class="logo-wrapper">
			<img src="../assets/logo.png" class="logo">
		</div>
		<img src="../assets/hero.jpg" class="background">
	</div>
</template>

<style>
.hero{
	width: calc(100% + 30px);
	display: block;
	overflow: hidden;
	margin: 0 -15px;
}
.logo-wrapper{
	position: absolute;
    margin-top: 30vh;
    width: 100%;
    text-align: center;
}
@media screen and (max-width: 1000px){
	.logo-wrapper img{
		max-width:90%;
	} 
}
.background{
	min-width: 100%;
	height:100vh;
}
</style>
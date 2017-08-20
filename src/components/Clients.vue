<template>
	<div class="row clients">
		<div class="content container text-center">
			<h2>_ourClients</h2>
					
			<p>We are proud to work with top clients.</p>
			<p>Check out a few of our clients</p>	

			<carousel 
				:scrollPerPage="true" 
				:autoplay="true"
				:perPage="3"
				:paginationEnabled="false">
				<slide>
					<img src="../assets/clients/belastingdienst.png">
				</slide>
				<slide>
					<img src="../assets/clients/boretti.png">
				</slide>
				<slide>
					<img src="../assets/clients/care-and-able.jpg">
				</slide>
				<slide>
					<img src="../assets/clients/macaw.png">
				</slide>
				<slide>
					<img src="../assets/clients/nn.jpg">
				</slide>
				<slide>
					<img src="../assets/clients/pon.jpg">
				</slide>
				<slide>
					<img src="../assets/clients/sa-logo.png">
				</slide>
				<slide>
					<img src="../assets/clients/sanoma.png">
				</slide>
				<slide>
					<img src="../assets/clients/zilveren-kruis.png">
				</slide>
			</carousel>		
		</div>
	</div>
</template>

<script>
import { Carousel, Slide } from 'vue-carousel'

export default{
	components:{
		Carousel,
		Slide
	}
}
</script>

<style>
.VueCarousel{
	position: relative;
	margin-top:30px;
	text-align: center;
	vertical-align: middle
}
.VueCarousel-slide{
	line-height: 120px;
}
.VueCarousel-slide img{
	display:inline-block;
}

</style>
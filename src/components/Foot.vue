<template>
	<div class="row footer theme-black">
		<div class="container footer--inner">
			<div class="row">
				<div class="col-sm-12 col-md-1 text-center logo">
					<img src="../assets/footer-logo.png" alt="Devmen">
				</div>
				<div class="col-sm-12 col-md-8 text-center links">
					<span class="link" v-if="!showPhone" @click="showPhone = true">Click to see the phone number</span>
					<a class="link" v-else href="tel:0850021011">0850021011</a>
					<span> | </span>
					<span class="link" v-if="!showMail" @click="showMail = true">Click to show email</span>
					<a class="link" v-else href="mailto:info@devmen.nl">info@devmen.nl</a>
					<span> | Curieweg 4C | Alphen aan den Rijn</span>
				</div>
				<div class="col-sm-12 col-md-3 text-center text-md-right contact">
					<h6>In a hurry? Call Jordi</h6>
					<ul class="list-inline">
						<li class="link" @click="showJordiPhone = true" v-if="!showJordiPhone">Click to see the phone number</li>
						<a class="link" v-else href="tel:+31628620688">+31628620688</a>
						<li class="link" @click="showJordiMail = true" v-if="!showJordiMail">Click to show email</li>
						<a class="link" v-else href="mailto:jordi@devmen.nl">jordi@devmen.nl</a>
						<li class="link"><a class="link" href="https://www.linkedin.com/in/jordiverzijden/" target="_blank">visit linkedin</a></li>
					</ul>
				</div>
			</div>
		</div>
	</div>
</template>

<script>

// Todo: Create function to switch active state of links.
export default{
	data(){
		return{
			showPhone: false,
			showMail: false,
			showJordiPhone: false,
			showJordiMail: false
		}
	}
}
</script>

<style>
a.link{
	color: #fbe108;
	cursor:pointer;
}
.link{
	color: #fbe108;
	cursor:pointer;
}
.theme-black .link:hover, .theme-black a:hover{
	color: #fff;
	text-decoration: underline;
}

.links{
	padding-top: 20px;
}

.footer{
	padding: 3rem 0;
}
</style>

<template>
	<div class="row footer theme-black">
		<div class="container footer--inner">
			<div class="row">
				<div class="col-sm-12 col-md-1 text-center logo">
					<img src="../assets/footer-logo.png" alt="Devmen">
				</div>
				<div class="col-sm-12 col-md-8 text-center links">
					<span class="link" :href="phone" @click="phone = '0850021011'">{{ phone }}</span>
					<span> | </span>
					<span class="link" :href="mail" @click="mail = 'info@devmen.nl'">{{mail}}</span>
					<span> | Curieweg 4C | Alphen aan den Rijn</span>
				</div>
				<div class="col-sm-12 col-md-3 text-center text-md-right contact">
					<h6>In a hurry? Call Jordi</h6>
					<ul class="list-inline">
						<li class="link" :href="jordiPhone" @click="jordiPhone = '+31628620688'">{{jordiPhone}}</li>
						<li class="link" :href="jordiMail" @click="jordiMail = 'jordi@devmen.nl'">{{jordiMail}}</li>
						<li class="link"><a href="https://www.linkedin.com/in/jordiverzijden/">visit linkedin</a></li>
					</ul>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
export default{
	data(){
		return{
			phone: "Click to see the phone number",
			mail: "Click to show email",
			jordiPhone: "Click to see the phone number",
			jordiMail: "Click to show email"
		}
	}
}
</script>

<style>
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
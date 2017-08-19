<template>
	<div class="row intro theme-grey">
		<ul>
			<li v-for="member in team">
				{{ member }}
			</li>
		</ul>
	</div>
</template>

<script>
	export default{
		data(){
			return{
				team:[
					{
						chris:{
							job: "Full-stack",
							picture: null,
							skill:[
								"PHP",
								"LARAVEL",
								"MAGENTO",
								"REACTJS",
								"ANGULARJS"
							]
						}
					},
					{
						jelle:{
							job: "Front-end",
							picture: null,
							skill:[
								"HTML & CSS",
								"TEAM LEAD",
								"MAGENTO",
								"REACTJS",
								"VUEJS"
							]
						}
					},
					{
						john:{
							job: "PHP",
							picture: null,
							skill:[
								"TEAM LEAD",
								"PHP",
								"MAGENTO",
								"ANGULARJS",
								"API INTERFACES"
							]
						}
					},
					{
						menno:{
							job: "PHP",
							picture: null,
							skill:[
								"PHP",
								"MAGENTO",
								"API INTERFACES",
								"JAVASCRIPT",
								"JAVA"
							]
						}
					},
					{
						carlo:{
							job: "Front-end",
							picture: null,
							skill:[
								"PHP",
								"MAGENTO",
								"API INTERFACES",
								"JAVASCRIPT",
								"JAVA"
							]
						}
					}
				]
			}
		}
	}
</script>

<style>

</style>
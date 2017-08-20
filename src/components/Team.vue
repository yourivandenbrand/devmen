<template>
	<div class="intro theme-grey container-fluid">
		<div class="content col-sm-12">
			<div class="row justify-center">
				<div v-for="member in team" class="col-sm-6 col-md-4 col-lg-3 col-xl-2">
					<div class="card">		
						<img :src="member.picture" class="card-img-top">
						<div class="card-header">
							<div class="card-text">{{member.job}}</div>
							<div class="card-label">{{member.name}}</div>
						</div>
						<div class="card-block">
							<div class="skilmatrix">
								<div v-for="(progress, label) in member.skills" class="progress-container">
									<div class="progress-bar" :style="{width: progress + '%'}">{{label}}</div>
								</div>
							</div>
						</div>
					</div>
				</div>	
			</div>	
		</div>
	</div>
</template>

<script>
import picChris from "../assets/team/chris.jpg"
import picJelle from "../assets/team/jelle.jpg"
import picJohn from "../assets/team/anon.jpg"
import picMenno from "../assets/team/menno.jpg"
import picCarlo from "../assets/team/carlo.jpg"
import picYouri from "../assets/team/youri.jpg"

export default{
	data(){
		return{
			team:[
				{						
					name: "Chris",
					job: "Full-stack",
					picture: picChris,
					skills:
						{"PHP": 100,
						"LARAVEL": 100,
						"MAGENTO": 100,
						"REACTJS": 80,
						"ANGULARJS": 70}
											
				},
				{						
					name: "Jelle",
					job: "Front-end",
					picture: picJelle,
					skills:{
						"HTML & CSS": 100,
						"TEAM LEAD": 100,
						"MAGENTO": 100,
						"REACTJS": 80,
						"VUEJS": 70
					}				
				},
				{						
					name: "John",
					job: "PHP",
					picture: picJohn,
					skills:{
						"TEAM LEAD": 100,
						"PHP": 100,
						"MAGENTO": 100,
						"ANGULARJS": 70,
						"API INTERFACES": 70
					}				
				},
				{						
					name: "Menno",
					job: "PHP",
					picture: picMenno,
					skills:{
						"PHP": 100,
						"MAGENTO": 100,
						"API INTERFACES": 80,
						"JAVASCRIPT": 70,
						"JAVA": 50
					}				
				},
				{						
					name: "Carlo",
					job: "Front-end",
					picture: picCarlo,
					skills:{
						"HTML & CSS": 100,
						"MAGENTO": 100,
						"WORDPRESS": 100,
						"USER EXPERIENCE": 70,
						"JAVASCRIPT": 50
					}						
				},
				{						
					name: "Youri",
					job: "Front-end",
					picture: picYouri,
					skills:{
						"HTML & CSS": 100,
						"JAVASCRIPT": 95,
						"GSAP": 95,
						"NODEJS": 80,
						"VUE 2": 70
					}						
				}
			]
		}
	}
}
</script>

<style>
.card{
	border: none;
	box-shadow: 0 0 10px 0 rgba(0,0,0,.2);
	margin-bottom: 1rem;
}

.card-img-top{
	border-radius: 50%;
    width: 100px;
    height: 100px;
    position: absolute;
    top: 80px;
    left: 10px;
}

.card-header{
	height: 133px;
	background-color: #000;
	margin-bottom: 50px;
}

.card-text{
	display: block;
	color: #fff;
	font-size: 1.3rem;
	text-align: left;
}

.card-block{
	-webkit-box-flex: 1;
	-webkit-flex: 1 1 auto;
	-ms-flex: 1 1 auto;
	flex: 1 1 auto;
	padding: 1.25rem;
}

.card-label{
	background: #fbe108;
	padding: 2px 10px;
	position: absolute;
	top: 118px;
	right: 0;
}

.justify-center{
	-webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
}

.progress-container{
	font-size:14px;
	margin-bottom:5px;
	background-color:#efefef;
}

.progress-bar{
	color:#000;
	padding:2px 5px;
	background-color:#cccccc;
	height:100%;
}

</style>
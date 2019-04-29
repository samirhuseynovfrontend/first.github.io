<template>
  <div id="about">
  	<div style="background-image:url(https://cdn.vuetifyjs.com/images/parallax/material.jpg)" class="white--text">
	  	<v-container>
	  	  <v-layout align-center class="mt-5" style="text-align:center">
	  	    <v-flex>
	  	    	<h3 class="display-3 mt-2">Welcome to the site About Us</h3>
	  	    	<p class="subheading">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
	  	    	tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
	  	    	quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
	  	    	consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
	  	    	cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
	  	    	proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
	  	    	<v-divider class="white"></v-divider>
	  	    	<h4 class="mt-5" style="font-size:25px">You welcome</h4>
	  	    	<v-btn class="ml-0 mr-0 white black--text" style="font-weight: bold; font-size: 20px; padding-left:50px; padding-right:50px">START</v-btn>
	  	    </v-flex>
	  	  </v-layout>
	  	</v-container>
  	</div>

  	<div>
	   	<v-container grid-list-xl class="mt-5 mb-5">
	  	  <v-layout row wrap align-start justify-end fill-height>
	  	  	<v-flex xs12 sm6 md4>
	  	  	  <v-card>
	  	  	  	<v-flex style="text-align:center">
	  	  	  		<v-icon class="minipi">fas fa-chart-bar</v-icon>
	  	  	  	</v-flex>
	  	  	  	<v-card-title style="text-align:center">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
	  	  	  	tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
	  	  	  	quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
	  	  	  	consequat. Excepteur sint occaecat cupidatat non
	  	  	  	proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</v-card-title>
	  	  	  </v-card>
	  	  	</v-flex>
	  	  	<v-flex xs12 sm6 md4>
	  	  	  <v-card>
	  	  	  	<v-flex style="text-align:center">
		  	  	  	<v-icon class="minipi">fas fa-user</v-icon>
	  	  	 	</v-flex>
	  	  	  	<v-card-title style="text-align:center">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
	  	  	  	tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
	  	  	  	quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
	  	  	  	consequat.</v-card-title>
	  	  	  </v-card>
	  	  	</v-flex>
	  	  	<v-flex xs12 sm6 md4>
	  	  	  <v-card>
	  	  	  	<v-flex style="text-align:center">
	  	  	  		<v-icon class="minipi">fas fa-clipboard-list</v-icon>
	  	  	  	</v-flex>
	  	  	  	<v-card-title style="text-align:center">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
	  	  	  	tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
	  	  	  	quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
	  	  	  	consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
	  	  	  	cillum dolore eu fugiat nulla pariatur.</v-card-title>
	  	  	  </v-card>
	  	  	</v-flex>
	  	  </v-layout>
	  	</v-container>
  	</div>

  	<div class="blue ligthen-2">
  		<v-container class="text-xs-center white--text pt-5 pb-5">
  			<v-layout>
  			  <p style="font-weight: bold; font-size:25px">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
  			  tempor incididunt ut labore et dolore magna aliqua.</p>
  			</v-layout>
  		</v-container>
  	</div>



  	<div>
  		<v-container>
  			<v-timeline align-top>
  				<v-timeline-item v-for="(item, i) in items" :key='i' :color="item.color" :icon="item.icon" fill-dot>
  					<v-card :color="item.color" dark>
  						<v-card-title class="title">Start your project</v-card-title>
  						<v-card-text class="white text--primary">
  							<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
  							tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
  							quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
  							consequat.</p>
  							<v-btn :color="item.color" class="mx-0" outline>
  								Start
  							</v-btn>
  						</v-card-text>
  					</v-card>
  				</v-timeline-item>
  			</v-timeline>
  		</v-container>
  	</div>
  	<v-divider></v-divider>
  	<div>
  		<v-container  class="text-xs-center mt-5 mb-5">
  		  <v-layout row wrap>
  		    <v-flex xs12 sm6 md6>
  		      <p class="mr-2" style="font-size:16px; font-weight: bold">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
  		      tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
  		      quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
  		      consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
  		      cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
  		      proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
  		    </v-flex>

  		    <v-flex xs12 sm6 md6>
  		      <img src="https://cdn.vuetifyjs.com/images/parallax/material.jpg" width="335px"  class="mr-1">
  		    </v-flex>
  		  </v-layout>
  		</v-container>
  	</div>

  	<my-footer></my-footer>
  	<router-view></router-view>
  </div>
</template>

<script>
import MyFooter from '@/components/myFooter'
	export default{
		data: () =>({
			items:[
				{
					color: 'red ligthen-2',
					icon: 'far fa-star'
				},
				{
					color: 'indigo ligthen-2',
					icon: 'fas fa-book'
				},
				{
					color: 'green ligthen-2',
					icon: 'fab fa-apple'
				},
				{
					color: 'blue ligthen-2',
					icon: 'fas fa-archive'
				}

			]
		}),
		components:{
    		MyFooter
  		}

	}
</script>

<style lang="stylus" scoped>
.minipi
	border-radius 50px
	border:2px solid grey
	width: 80px
	height:80px
	font-size: 45px
</style>
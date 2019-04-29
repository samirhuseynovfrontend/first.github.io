<template>
  <div>
  	<div><!--footer-->
  		<v-footer height="auto" dark>
  			<v-card title flat class="dark text-xs-center white--text lighten-1">
  				<v-card-text class="green">
  					<v-btn v-for="icon in icons" :key="icon" class="mx-3 white--text" icon>
  						<v-icon size="24px">{{icon}}</v-icon>
  					</v-btn>
  				</v-card-text>
  				<v-card-text class="white--text pt-0 green">
	  				Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
	  				tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
	  				quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
	  				consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
	  				cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
	  				proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
	  			</v-card-text>
	  			<v-divider></v-divider>
	  			<v-card-text class="white--text">
	  				&copy;2019 - <strong>SAMIR</strong>
	  			</v-card-text>
  			</v-card>
  		</v-footer>
  	</div>
  </div>
</template>

<script>
	export default{
		data(){
			return{
				icons:[
					'fab fa-facebook',
			        'fab fa-twitter',
			        'fab fa-google-plus',
			        'fab fa-linkedin',
			        'fab fa-instagram'
				]
			}
		}
	}
</script>

<style lang="stylus" scoped>

</style>
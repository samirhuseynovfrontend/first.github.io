<template>
	<div>
		<v-navigation-drawer v-model="drawer" absolute temporary>
		   <v-list>
		   		<v-list-tile avatar>
		   		  	<v-list-tile-content>
            			<v-list-tile-title style="font-size:25px; font-weight: bold">StartUp</v-list-tile-title>
         	 		</v-list-tile-content>
		   		</v-list-tile>
		   </v-list>
		   <v-divider></v-divider>
		   <v-list>
		   		<v-list-tile v-for="item in menuItems" :key="item.title" @click="" :to="item.url">
		   		  	<v-list-tile-content>
            			<v-list-tile-title>{{ item.title }}</v-list-tile-title>
          			</v-list-tile-content>
		   		</v-list-tile>
		   			<my-dialog></my-dialog>
		   </v-list>
		</v-navigation-drawer>
	    <v-toolbar color="blue" dark fixed>
	    	<router-link to="/" tag="span" style="cursor:pointer">
	    		<v-toolbar-title  v-text="'StartUp'"></v-toolbar-title>
	    	</router-link>
	    	<v-spacer></v-spacer>
	    	<v-toolbar-items class="hidden-sm-and-down">
	    		<v-btn flat v-for="item in menuItems" :to="item.url" :key="item.title">{{item.title}}</v-btn>
	    		<my-dialog></my-dialog>
	    	</v-toolbar-items>
	    	<v-toolbar-side-icon class="hidden-md-and-up" @click.stop="drawer = !drawer"></v-toolbar-side-icon>
	    </v-toolbar>
	</div>
</template>

<script>
import MyDialog from '@/components/myDialog'
export default {
	data: ()=>({
		drawer: null
	}),
	computed:{
			menuItems(){
				return[
					{title: 'Home', url:'/'},
					{title: 'Gallery', url:'/gallery'},
					{title: 'About', url:'/about'}
				]
			}
	},
	components:{
   	 	MyDialog
  	}
}
</script>

<style lang="stylus" scoped>

</style>
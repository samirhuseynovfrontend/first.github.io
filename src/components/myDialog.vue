<template>
	
		<v-dialog
      v-model="dialog"
      width="500"
    >
      <template v-slot:activator="{ on }">
        <v-btn flat
          v-on="on"
        >
          Contact
        </v-btn>
      </template>

      <v-card>
        <v-card-title
          class="headline grey lighten-2"
          primary-title
        >
          Log In
        </v-card-title>

        <v-card-text>
          <v-form>
          	<v-text-field label="Name" required></v-text-field>
          	<v-text-field label="Email" required></v-text-field>
          	<div class="text-xs-center">
          	  <v-btn>Start</v-btn>
            </div>
          </v-form>
        </v-card-text>

        <v-divider></v-divider>

        <v-card-actions>
          <v-spacer></v-spacer>
          <v-btn
            color="primary"
            flat
            @click="dialog = false"
          >
            Exit
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
	
</template>

<script>

export default {
	data () {
      return {
        dialog: false
      }
    }
}
</script>

<style lang="stylus" scoped>

</style>
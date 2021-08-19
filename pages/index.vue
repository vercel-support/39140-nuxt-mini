<template>
  <div>
	  Homepage.
	  <br>
	  Visiting <nuxt-link :to="`https://${sub}.loginhook.com`">{{sub}}.loginhook.com</nuxt-link> should show the message: "Hello user {{sub}}"
  </div>
</template>

<script>
export default {
	data(){
		return {
			sub:''
		}
	},
	mounted(){
		this.sub = + new Date()
	}
}
</script>

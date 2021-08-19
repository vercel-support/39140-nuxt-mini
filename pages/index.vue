<template>
  <div>
	  Homepage.
	  <br>
	  Visiting <a :href="`https://${sub}.loginhook.com`">{{sub}}.loginhook.com</a> should show the message: "Hello user {{sub}}"
  </div>
</template>

<script>
export default {
	data(){
		return {
			sub:''
		}
	},
	created(){
		this.sub = + new Date()
	}
}
</script>

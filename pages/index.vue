<template>
  <div>
	  Homepage.
	  <br>
	   <br>
	  Visiting <a :href="`https://${sub}.loginhook.com`">{{sub}}.loginhook.com</a> it should show the message: "Hello user {{sub}}"
	  (The content of <a :href="`https://loginhook.com/user/${sub}`">https://loginhook.com/user/{{sub}}</a>)
	  <br>
	   <br>
	  Instead it shows this page (The homepage)
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

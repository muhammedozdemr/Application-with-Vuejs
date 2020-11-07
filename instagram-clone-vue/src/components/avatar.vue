<template>
	<figure class="avatar">
		<img :src="src" :alt="alt" :width="size" :height="size">
		
	</figure>	
</template>

<script>
	export default{
		name:"Avatar",
		props:{
			src:{
				type:String,
				default:
				"https://instagram.fasr1-1.fna.fbcdn.net/v/t51.2885-19/s150x150/118699616_346321020066427_3802221597371669863_n.jpg?_nc_ht=instagram.fasr1-1.fna.fbcdn.net&_nc_ohc=2jNkTdyt3UIAX9tp57L&oh=251243508900295690b5917c66726722&oe=5FCFA674"
			},
			alt:{
				type:String
			},
			size:{
				type:Number
			}
		}
	}
</script>

<style scoped>
	.avatar{
		padding: 2px;
		border-radius:999px;
		display: inline-flex;
		background:linear-gradient(219deg,rgba(184,63,140,1)0%,rgba(237,158,90,1)100%);
		img{
			border-radius:inherit;
			border:2px solid white;
		}
	}
</style>
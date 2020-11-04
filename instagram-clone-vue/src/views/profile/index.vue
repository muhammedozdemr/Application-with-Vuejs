<template>
  <div class="home">
 
    <CustomText tag="h1">Profile</CustomText>
    <CustomText tag="p">Lorem ipsum, dolor sit amet, consectetur adipisicing elit. Blanditiis, cumque, velit. Labore mollitia molestiae ratione eligendi, quae. Voluptatem molestias sunt tempore odit ex, dignissimos consequatur praesentium ut, distinctio, nobis doloribus.</CustomText>

    <div id="nav">
      <router-link to="/profile">Post</router-link> |
      <router-link to="/profile/igtv">IGTV</router-link> |
      <router-link to="/profile/save">Save</router-link> |
      <router-link to="/profile/tag">Tag</router-link>
    </div>
    
    <router-view />
  </div>
</template>

<script>
	import CustomText from '@/components/CustomText'
  

export default {
  name: "Profile",
  components:{
  	CustomText
   
  }
};
</script>

<style>
	
</style>
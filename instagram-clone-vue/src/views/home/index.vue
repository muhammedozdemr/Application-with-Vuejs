<template>
  <div class="home">

    <div class="timeline"> 


    <Post />

    <br>
    <br>
    <br>
    <br>
    <br>
    <br>
    </div>
    <div class="sidebar">
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quasi necessitatibus deserunt sit eos laudantium praesentium, excepturi aliquid nisi, odio. Ut magnam maxime itaque impedit, qui, molestiae eos assumenda sit est!</p>

    </div>

   
  </div>
</template>

<script>
  import Post from "@/components/Post"
	
export default {
  name: "Home",
  components:{
    Post
  }
  
};
</script>

<style>
	.home{
    max-width: 605px;
    margin-left: auto;
    margin-right: auto;

    @media(--t){
    max-width:none;
    display: grid;
    grid-template-columns: 1fr 295px;
    grid-gap: 30px;

    }
  }
  .sidebar{
    display: none;
    @media(--t){
    display: block;
    }
  }

</style>
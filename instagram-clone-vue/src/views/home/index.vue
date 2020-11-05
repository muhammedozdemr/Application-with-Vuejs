<template>
  <div class="home">

    <div class="timeline"> 

    <h1>Home</h1>
    <CustomText class="a1" tag="p">Merhaba Dünya</CustomText>
    <CustomText class="a2" tag="p" size="small">Merhaba Dünya</CustomText>
    <CustomText class="a3" tag="p" size="xsmall">Merhaba Dünya</CustomText>
    <CustomText tag="p" size="xxsmall">Merhaba Dünya</CustomText>
    <IconHome width="60" height="60" />
    <p>Lorem ipsum dolor sit, amet consectetur, adipisicing elit. Suscipit molestiae ab eligendi. Aut, reprehenderit provident vitae sit pariatur magnam id neque perspiciatis quia, tempora amet, incidunt expedita temporibus ullam fugit.</p>
    <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quod a unde sint necessitatibus facere eum distinctio deserunt maiores eos veritatis, inventore corporis, accusantium animi iure quae harum porro expedita optio.</p>
    </div>
    <div class="sidebar">
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quasi necessitatibus deserunt sit eos laudantium praesentium, excepturi aliquid nisi, odio. Ut magnam maxime itaque impedit, qui, molestiae eos assumenda sit est!</p>

      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quasi necessitatibus deserunt sit eos laudantium praesentium, excepturi aliquid nisi, odio. Ut magnam maxime itaque impedit, qui, molestiae eos assumenda sit est!</p>
    </div>

   
  </div>
</template>

<script>
	import CustomText from '@/components/CustomText'
  import IconHome from '../../icons/home.svg'

export default {
  name: "Home",
  components:{
  	CustomText,
    IconHome
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
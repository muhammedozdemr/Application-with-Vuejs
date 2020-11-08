<template>
	<div class="post">
		<!--Header-->
		<header class="header section">
			
			<div class="header-author">
				<Avatar :size="40"/>
				<div class="header-author-info">
					<div><CustomText tag="b">_mozdemr</CustomText></div>
					
					<div><CustomText size="xsmall">Elazığ, Turkey</CustomText></div>
				</div>
			</div>
			<div class="header-more">
				<button type="button">
					<IconMore />
				</button>
			</div>
		</header>

		<!--Media-->
		<div class="post-media">
			<img src="https://instagram.fasr1-1.fna.fbcdn.net/v/t51.2885-15/fr/e15/s1080x1080/123813995_3042730975828189_8441045778176073254_n.jpg?_nc_ht=instagram.fasr1-1.fna.fbcdn.net&_nc_cat=1&_nc_ohc=zq9gOIfuECkAX-ateQl&oh=879da6a5b5d7fba9c652c152624b164f&oe=5FD183D8" alt="">
		</div>
		<!--Actions-->
		<div class="action-buttons section">
			<button type="button">
				<IconLike />
			</button>
			<button type="button">
				<IconComment />
			</button>
			<button type="button">
				<IconDirect />
			</button>
			<button class="action-save" type="button">
				<IconSave />
			</button>
		</div>

		<!--ViewCount-->
		<div class="view-count section">
			<CustomText tag="b">1.907 beğenme</CustomText>
		</div>

		<!--CommentList-->

		<!--Datetime-->

		<!--CommentForm-->
		
	</div>
</template>

<script>
	import Avatar from "@/components/Avatar"
	import CustomText from "@/components/CustomText"
	import IconMore from "@/icons/more.svg"
	import IconLike from "@/icons/like.svg"
	import IconComment from "@/icons/comment.svg"
	import IconDirect from "@/icons/direct.svg"
	import IconSave from "@/icons/save.svg"
	export default{
		name:"Post",
		components:{
			Avatar,
			CustomText,
			IconMore,
			IconLike,
			IconComment,
			IconDirect,
			IconSave
		}
	}
</script>

<style scoped>
	.post{
		border-radius: 3px;
		border:1px solid rgb(var(--b6a));

	}
	.section{
		padding-left: 16px;
		padding-right: 16px;
	}
	.header{
		height: 60px;
		display: flex;
		align-items: center;
		&-author{
			display: flex;
			align-items: center;
			&-info{
				margin-left: 8px;
			}
		}

		&-more{
			margin-left: auto;
		}
	}
	.action-buttons{
		height: 45px;
		display: flex;
		align-items: center;

		button{
			margin-right: 16px;
		}
		.action-save{
			margin-left: auto;
			margin-right: 0;
		}
	}
</style>
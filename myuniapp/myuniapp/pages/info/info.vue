<template>
	<view class="content">
		<view class="title">
			{{title}}
		</view>
		<view class="art-content">
			<rich-text :nodes="content"></rich-text>
		</view>
	</view>
</template>

<script>
	export default {
		data(){
			return{
				title:'',
				content:'',
			}
		},
		onLoad:function(e){
			var that=this;
			console.log(e.newsid)
			uni.request({
				url: 'https://unidemo.dcloud.net.cn/api/news/36kr/'+e.newsid,
				method: 'GET',
				data: {},
				success: res => {
					that.title=res.data.title;
					that.content=res.data.content
				},
				fail: () => {},
				complete: () => {}
			});
		}
	}
</script>

<style>
.content{
	padding: 10upx 2%;
	width: 96%;
	flex-wrap: wrap;
}
.title{
	line-height: 2em;
	font-weight: bold;
	font-size: 38upx;
}
.art-content{
	line-height: 2em;
}
</style>

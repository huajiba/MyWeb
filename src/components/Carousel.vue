<template>
	<div>
		<div class="container">
			<div id="carouselExampleCaptions" class="carousel slide" data-ride="carousel">
				<ol class="carousel-indicators">
				<li data-target="#carouselExampleCaptions" data-slide-to="0" class="active"></li>
				<li data-target="#carouselExampleCaptions" data-slide-to="1"></li>
				<li data-target="#carouselExampleCaptions" data-slide-to="2"></li>
				<li data-target="#carouselExampleCaptions" data-slide-to="3"></li>
				</ol>
				<div class="carousel-inner">
				<div class="carousel-item active">
					<img :src="imgSrc1" class="d-block w-100" alt="...">
				</div>
				<div class="carousel-item" v-for="x in imgSrcArr">
					<img :src="x" class="d-block w-100" alt="...">
				</div>
				
				</div>
				<button class="carousel-control-prev" type="button" data-target="#carouselExampleCaptions" data-slide="prev">
				<span class="carousel-control-prev-icon" aria-hidden="true"></span>
				<span class="sr-only">Previous</span>
				</button>
				<button class="carousel-control-next" type="button" data-target="#carouselExampleCaptions" data-slide="next">
				<span class="carousel-control-next-icon" aria-hidden="true"></span>
				<span class="sr-only">Next</span>
				</button>
			</div>
		</div>
	</div>
</template>

<script>
	// JS代码 Vue代码
	// 选项式
	export default{
		data(){
			return {
				imgSrc1:"http://p1.music.126.net/o7PwZZl6b6ESqjmn5D_87w==/109951169068264440.jpg?imageView&quality=89",
				imgSrcArr: ['http://p1.music.126.net/evX6rhl-LtJbwmGrhTzCmg==/109951169068350203.jpg?imageView&quality=89',
							'http://p1.music.126.net/IECDissztdVHfr71HEln9Q==/109951169068349921.jpg?imageView&quality=89',
							'http://p1.music.126.net/Em6qlrjo5adWob44PwAVww==/109951169068422140.jpg?imageView&quality=89']
			}
		},
		methods:{
			
		}
	}
	//组合式 [添加setup]

</script>

<style>
</style>
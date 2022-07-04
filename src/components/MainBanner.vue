<template>
	<!-- <div class="container"> -->

		<div id="banner1" class="bannerRotativo">1</div>
		<!-- <img src="/img/banner-2.jpg" id="banner1" class="bannerRotativo">
		<img src="/img/banner-3.jpg" id="banner1" class="bannerRotativo">
		<img src="/img/banner-4.jpg" id="banner1" class="bannerRotativo">
		<img src="/img/banner-5.jpg" id="banner1" class="bannerRotativo">
		<img src="/img/banner-6.jpg" id="banner1" class="bannerRotativo"> -->

		<!-- <div class="bannerRotativo">
			<div id="banner2" class="banner">2</div>
			<div id="banner3" class="banner">3</div>
			<div id="banner4" class="banner">4</div>
		</div> -->

		<div class="btn-group" style="margin: 0 auto; position: relative;">
			<div style="position: absolute; bottom: 10px; left: -200px">
				<button id="botaoBanner1" type="button" class="botaoBanner btn btn-default" data-banner="1">Banner 1</button>
				<button id="botaoBanner2" type="button" class="botaoBanner btn btn-default" data-banner="2">Banner 2</button>
				<button id="botaoBanner3" type="button" class="botaoBanner btn btn-default" data-banner="3">Banner 3</button>
				<button id="botaoBanner4" type="button" class="botaoBanner btn btn-default" data-banner="4">Banner 4</button>
				<button id="botaoBanner5" type="button" class="botaoBanner btn btn-default" data-banner="4">Banner 5</button>
				<button id="botaoBanner6" type="button" class="botaoBanner btn btn-default" data-banner="4">Banner 6</button>
			</div>
		</div>
	<!-- </div> -->
</template>

<script>
export default {
	name: 'MainBanner',

	methods: {

		/* incrementarValor() {
			var iterator = 0;
			var quantidadeDeBanners = $(".banner").length;
			var banner = iterator%quantidadeDeBanners;
			var timer = null;
			mostrarBanner(banner+1);
			iterator = iterator+1;
		},
		ligar() {
			timer = setInterval(incrementarValor, 2000);
		},
		desligar() {
			clearInterval(timer);
		},
		mostrarBanner(id){
			$(".banner").removeClass('ativo');
			$("#banner"+id).addClass('ativo');

			$(".botaoBanner").removeClass('btn-primary');
			$("#botaoBanner"+id).addClass('btn-primary');
		},
		$(".botaoBanner").on("click", function() {
			var idBanner = $(this).attr('data-banner');
			mostrarBanner(idBanner);
			iterator = idBanner;
			desligar();

			setTimeout(function(){ ligar(); }, 3000)
		}),
		$(".bannerRotativo").on("mouseover", function() {
			desligar();
		}),
		$(".bannerRotativo").on("click mouseout", function() {
			ligar();
		}),

		ligar() */
	}
}
</script>

<style lang="scss" scoped>
.bannerRotativo {
	width: 100%;
	height: 350px;
	/* margin: 30px; */
	/* border: 1px solid black; */
	background-image: url("../../public/img/banner-3.jpg");
	margin: 0 auto;
	align-items: center;
	background-position: 0px;
	background-size: cover;
	display: flex;
	justify-content: flex-start;
}

.banner {
	background-color: #ddd;
	height: 100%;
	text-align: center;
	line-height: 90px;
	display: none;
}
.banner.ativo {
	display: block;
}

.btn-group {
	left: 50%;
	margin: 30px auto 0 -130px;
}
</style>

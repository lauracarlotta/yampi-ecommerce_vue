<template>
	<header>
		<div class="container">
			<div id="yampi-header">
				<router-link to="/">
					<img class="yampi-logo__header" src="https://i.ibb.co/Vj7LVmk/yampi-logo.png" alt="">
				</router-link>
				
				<div id="yampi-header__search">
					<input id="input-search__main" type="search" placeholder="O que você está procurando? ">
					<i class="fa-solid fa-magnifying-glass"></i>
				</div>
				<div id="yampi-header__shopping">
					<i class="fa-solid fa-cart-shopping"></i>
					<div>3 itens</div>
					<div>R$ 2.578,70</div>
				</div>
			</div>
			<nav>
				<div id="yampi-nav">
					<router-link class="yampi-nav__link" to="/">Electronics</router-link>
					<router-link class="yampi-nav__link" to="/">Jewelery</router-link>
					<router-link class="yampi-nav__link" to="/">Men's Clothing</router-link>
					<router-link class="yampi-nav__link" to="/">Women's Clothing</router-link>
				</div>
			</nav>
		</div>
	</header>
	<main>
		<router-view />
	</main>
	<footer>
		<div class="container">
			<div id="yampi-footer">
				<img class="yampi-logo__footer" src="https://i.ibb.co/Vj7LVmk/yampi-logo.png" alt="">

				<div class="yampi-ul">
					<ul class="yampi-ul__footer">
						<strong>Institucional</strong>
						<li><a href="#"> Quem somos </a></li>
						<li><a href="#"> Política de privacidade </a></li>
						<li><a href="#"> Política de compra </a></li>
						<li><a href="#"> Política de troca e devolução </a></li>
						<li><a href="#"> Nossas lojas </a></li>
					</ul>

					<ul class="yampi-ul__footer">
						<strong>Ajuda</strong>
						<li><a href="#"> Fale conosco </a></li>
						<li><a href="#"> Perguntas frequentes </a></li>
					</ul>
				</div>
			</div>
		</div>
	</footer>
</template>

<style lang="scss" src="./style.scss"/>

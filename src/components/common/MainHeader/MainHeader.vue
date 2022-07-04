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
</template>

<script>
export default {
	name: 'MainHeader',
}
</script>

<style lang="scss" src="./MainHeader.scss" scoped/>

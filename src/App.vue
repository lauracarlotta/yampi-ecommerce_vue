<template>
	<header>
		<div class="container">
			<div id="yampi-header">
				<img class="yampi-logo" src="https://i.ibb.co/Vj7LVmk/yampi-logo.png" alt="">
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
			<div>
				<img src="https://i.ibb.co/Vj7LVmk/yampi-logo.png" alt="">
			</div>

			<div>
				<ul>Institucional
					<li>Quem somos</li>
					<li>Política de privacidade</li>
					<li>Política de compra</li>
					<li>Política de troca e devolução</li>
					<li>Nossas lojas</li>
				</ul>
			</div>

			<div>
				<ul>Ajuda
					<li>Fale conosco</li>
					<li>Perguntas frequentes</li>
				</ul>
			</div>
		</div>
	</footer>
</template>

<style lang="scss">
#app {
	font-family: Avenir, Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #2c3e50;
}

* {
	box-sizing: border-box;
	font-family: Helvetica, sans-serif;
	margin:0;
	padding: 0;
}

header {
	background-color: #f3f4f6;
	border-bottom: .25rem solid #dedaf1;

	.container {
		margin: 0 auto;
		width: 1120px;

		#yampi-header {
			align-items: center;
			display: flex;
			justify-content: space-between;

			i {
				color: #725bc2;
			}

			.yampi-logo {
				width: 200px;
			}

			#yampi-header__search {

				#input-search__main {
					border-radius: .5rem;
					border: 2px solid #8e7dcf;
					padding: .75rem 1.5rem;
					width: 550px;
					max-width: 700px;
				}

				i {
					position: relative;
					top: 4px;
					right: 36px;
					cursor: pointer;
					font-size: 1.5rem;
				}

			}

			#yampi-header__shopping {
				background-clip: #efecf8;
				padding: 1rem;
				margin-top: 1rem;
				border-radius: 1rem;
				display: flex;
				flex-direction: column;
				box-shadow: 0 10px 15px -3px rgba(0,0,0,0.1),
							0 4px 6px -2px rgba(0,0,0,0.05);
				cursor: pointer;
				transition: all 500ms ease;

				i {
					margin-bottom: 1rem;
					font-size: 2rem;
				}

				&:hover {
					background-color: #dedaf1;
				}
			}
		}

		nav {
			margin-top: 2rem;

			#yampi-nav {
			display: flex;
			align-items: stretch;
			flex-direction: row;
			justify-content: space-between;
			padding: 0 1rem;

			.yampi-nav__link {
				color: #374151;
				text-decoration: none;
				text-transform: uppercase;
				font-weight: bolder;
				padding: 1rem 0;
				width: 25%;

				&:hover {
					border-radius: 1rem 1rem 0 0;
					background-color: #dedaf1;
				}
			}
		}
		}
	}
}

</style>

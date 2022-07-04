<template>
	<MainHeader />

	<main>
		<router-view />
	</main>

	<MainFooter />
</template>

<script>
import MainHeader from './components/common/MainHeader/MainHeader.vue';
import MainFooter from './components/common/MainFooter/MainFooter.vue';

export default {
	name: 'App',

	components: {
		MainHeader,
		MainFooter,
	}
}
</script>

<style lang="scss" src="./style.scss"/>

<template>
	<div class="home">
		<MainBanner />
		<!-- <img alt="Vue logo" src="/img/logo.jpg" /> -->
	</div>
</template>

<script>
import MainBanner from '../components/MainBanner.vue';

export default {
	name: "HomeView",

	components: {
		MainBanner,
	}
};
</script>

<template>
	<div class="home">
		<NavbarHeader/>
	</div>
</template>

<script>
// eslint-disable-next-line import/no-unresolved
import NavbarHeader from '@/components/NavbarHeader/NavbarHeader.vue';

export default {
	name: 'HomeView',
	components: {
		NavbarHeader,
	},
};
</script>

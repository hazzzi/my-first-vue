<template>
	<div>
		<Header />
		<article class="wrap">
			<Box color="blue" />
			<Box color="purple" />
			<Box />
			<Box />
			<Box />
		</article>
	</div>
</template>

<script>
import Header from './components/Header';
import Box from './components/Box';

export default {
	name: 'App',
	components: {
		Header,
		Box,
	},
};
</script>

<style scoped>
.wrap {
	display: flex;
}
</style>

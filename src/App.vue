<template>
	<div>
		<Header />
		<article class="wrap">
			<Menu />
			<Content />
		</article>
	</div>
</template>

<script>
import Header from './components/Header';
import Content from './components/Content';
import Menu from './components/Menu';

export default {
	name: 'App',
	components: {
		Header,
		Content,
		Menu,
	},
};
</script>

<style scoped>
.wrap {
	display: flex;
}
</style>

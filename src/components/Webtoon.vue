<template>
	<div>
		<h2>Webtoon</h2>
		<ul class="wrap">
			<li
				class="item"
				v-for="({ name, link, img }, idx) in items"
				:key="{ idx }"
			>
				<a :href="link" target="_blank">
					<img :src="img" />
					<span class="title">제목: {{ name }}</span>
				</a>
			</li>
		</ul>
	</div>
</template>

<script>
export default {
	props: {
		items: { type: Array, default: () => [] },
	},
};
</script>

<style scoped>
h2 {
	text-align: center;
}

a {
	list-style: none;
	text-decoration: none;
}

li {
	list-style: none;
}

.wrap {
	max-width: 450px;
	width: 100%;
	margin: 0 auto;
}

.item {
	border-bottom: 1px solid #ebebeb;
	margin-bottom: 25px;
}

.title {
	display: inline-block;
	font-size: 18px;
	font-weight: bold;
	color: #000;
	padding: 20px 15px;
}

img {
	width: 100%;
	background: #ebebeb;
	border-radius: 4px;
}
</style>

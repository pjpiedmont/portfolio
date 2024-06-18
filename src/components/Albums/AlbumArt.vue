<script setup lang="ts">
defineProps<{
	src: string;
	alt: string;
}>();
</script>

<!----------------------------------------------------------------------------->

<template>
	<div class="container p-0">
		<img :src="src" :alt="alt">
	</div>
</template>

<!----------------------------------------------------------------------------->

<style scoped lang="scss">
@import '@/assets/scss/variables/colors.scss';

div {
	overflow: hidden;
	border: 1px solid var(--accent-bg-color);
	border-radius: 10%;
}

img {
	max-width: 100%;
	max-height: 100%;
	overflow: hidden;
	border: 1px solid $color-primary;
	border-radius: 10%;
}
</style>

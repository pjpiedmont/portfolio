<script setup lang="ts">
import AlbumArt from './AlbumArt.vue';

defineProps<{
	albumArtSrc?: string;
	albumArtAlt?: string;
}>();
</script>

<!----------------------------------------------------------------------------->

<template>
	<div class="row p-0">
		<div class="col-lg-6 p-0 border-top">
			<div v-if="albumArtSrc" class="container p-4 p-lg-5">
				<AlbumArt :src="albumArtSrc" :alt="albumArtAlt" />
			</div>
		</div>
	</div>
</template>

<!----------------------------------------------------------------------------->

<style scoped lang="scss"></style>
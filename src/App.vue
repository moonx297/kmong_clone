<template>
	<div id="app">
		<HeaderArea />
		<router-view />
		<FooterArea />
	</div>
</template>

<script>
import HeaderArea from '@/components/header-area.vue'
import FooterArea from '@/components/footer-area.vue'
import '@/assets/css/common.css'

export default {
	components: {
		HeaderArea,
		FooterArea,
	},
}
</script>

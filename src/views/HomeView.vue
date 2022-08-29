<template>
	<div class="container">
		<h3 class="subtitle">관심사가 비슷한 회원들이 본 서비스</h3>
		<ContentArea />
	</div>
</template>

<script>
import ContentArea from '@/components/content-area.vue'
export default { components: { ContentArea } }
</script>

<style scoped>
.subtitle {
	margin-bottom: 20px;
	margin-top: 20px;
	font-weight: 800;
}
</style>

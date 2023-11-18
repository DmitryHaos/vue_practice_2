<template>
	<h1>Notification Center</h1>
	<notification-message header="You are eligible for a reward">
		<p>Go to the <b>special offers</b> page to see now.</p>
	</notification-message>
	<notification-message header="Information" type="info">
		<p>Test text Information</p>
	</notification-message>
	<notification-message header="Error 404" type="error">
		<p>The file was not found</p>
	</notification-message>
	<notification-message type="success">
		<b>Success</b>
	</notification-message>	
</template>

<script>
	import NotificationMessage from '@/components/NotificationMessage.vue'
	export default {
		name: 'App',
		components: {
			NotificationMessage
		}
	}
</script>

<style>
	#app {
		font-family: Avenir, Helvetica, Arial, sans-serif;
		-webkit-font-smoothing: antialiased;
		-moz-osx-font-smoothing: grayscale;
		text-align: center;
		color: #2c3e50;
		margin-top: 60px;
	}
</style>

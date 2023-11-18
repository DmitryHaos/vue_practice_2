<template>
    <div class="ui message" :class="type" v-if="active">
		<i class="close icon" @click="close"></i>
		<div class="header">
			{{header}}
		</div>
		<slot></slot>
	</div>
</template>

<script>
	export default {
		name: 'NotificationMessage',
		props: {
			type : {
				type: String
			},
			header: {
				type: String
			}
		},
		data(){
			return {
				active: true
			}
		},
		methods:{
			close(){
				this.active = false;
			}
		}
	}
</script>
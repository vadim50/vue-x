<template>
	<div>
		<button class="btn btn-success" @click="updateCounter(1)">+1</button>
		<button class="btn btn-danger" @click="updateCounter(-1)">-1</button>
	</div>
</template>
<script>
	export default {
		methods: {
			updateCounter(val){
				//this.$emit('counterUpdated', val)
				this.$store.state.counter += val
			}
		}
	}
</script>
<template lang="pug">
div(@click="changeName()").
	Hello, {{ name }}.
</template>

<script>
export default {
	name : 'example',
	data() {
		return {
			name : 'world'
		};
	},
	methods : {
		changeName() {
			this.name = 'foobar';
		}
	}
};
</script>

<style lang="sass" scoped>
div
	font-weight: bold
</style>
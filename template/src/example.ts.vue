<template lang="pug">
div(@click="changeName()").
	Hello, {{ name }}.
</template>

<script lang="ts">
import Vue from 'vue'
import Component from 'vue-class-component'

@Component({ name: 'example' })
export default class Example extends Vue {
	name = 'world'

	changeName() {
		this.name = 'foobar'
		console.log(this.name)
	}
}
</script>

<style lang="sass" scoped>
div
	font-weight: bold
</style>
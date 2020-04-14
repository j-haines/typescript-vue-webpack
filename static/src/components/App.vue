<template>
	<div @click="hello">Hello, {{ name }}!</div>
</template>

<script lang="ts">
import {Vue, Component} from "vue-property-decorator"

@Component
export default class App extends Vue {
	// undecorated property will be packed in `data` option
	name = "world"

	// undecorated method will be packed in `methods` option
	hello() {
		alert("Hello, " + this.name)
	}
}
</script>

<style>

</style>

<template>
	<div class="home">
		<TelemetryBox style="--order: 1" />
		<TelemetryBox style="--order: 2" />
		<TelemetryBox style="--order: 3" />
		<TelemetryBox style="--order: 4" />
		<TelemetryBox style="--order: 5" />
		<TelemetryBox style="--order: 6" />
		<TelemetryBox style="--order: 7" />
		<TelemetryBox style="--order: 8" />
		<TelemetryBox style="--order: 9" />
		<TelemetryBox style="--order: 10" />
		<TelemetryBox style="--order: 11" />
		<TelemetryBox style="--order: 12" />
	</div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import TelemetryBox from "@/components/TelemetryBox.vue"; // @ is an alias to /src

@Options({
	components: {
		TelemetryBox
	}
})
export default class Home extends Vue {}
</script>

<style scoped lang="scss"></style>

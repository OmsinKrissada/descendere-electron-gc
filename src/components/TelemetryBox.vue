<template>
	<div class="box">
		<div class="bar">
			<div class="left">
				<h2>TELEMETRY CONTROL</h2>
			</div>

			<div class="right">
				<div class="group">
					<p class="title">Total Packet Count:</p>
					<p class="code">{{ total_pkg }}</p>
				</div>
				<div class="group">
					<p class="title">Last Command:</p>
					<p class="code">{{ last_cmd }}</p>
				</div>
			</div>
		</div>
		<div id="input"></div>
	</div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({})
export default class TelemetryBox extends Vue {
	total_pkg = 0;
	last_cmd = "-";
}
</script>

<style scoped lang="scss"></style>

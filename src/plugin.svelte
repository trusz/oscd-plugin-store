<script lang="ts">
	import * as pckg from "../package.json";
	import "./app.css"
	
	// Inputs
	export let doc: XMLDocument | undefined;
	export let editCount: number

	export function run(){
		console.log("Plugin is running");
	}
</script>

{#if doc}
	<h2>Welcome to oscd-plugin-store</h2>
{/if}

<input type="hidden" name="package-name" value={pckg.name} />
<input type="hidden" name="package-version" value={pckg.version} />

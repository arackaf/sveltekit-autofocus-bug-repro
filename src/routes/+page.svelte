<script lang="ts">
  import Component from "./Component.svelte";

  let value = 0;
  let update = () => (value = value + 1);
</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

<Component {value} {update} />

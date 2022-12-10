<script lang="ts">
  export let value: any;
  export let update: any;
</script>

<form>
  <input autofocus />
</form>

{value}

<br />
<a on:click={update} on:keypress={() => {}}>Bad link - no href (will refocus)</a>

<br />
<br />
<a href="https://xhamster.com" on:click={(e) => e.preventDefault()} on:keypress={() => {}}>
  Good link - has href with prevent default (will not refocus)</a
>

<br />
<br />
<button on:click={update} on:keypress={() => {}}>Update (will not refocus - which is correct)</button>

<style>
  a {
    text-decoration: underline;
    cursor: pointer;
  }
</style>

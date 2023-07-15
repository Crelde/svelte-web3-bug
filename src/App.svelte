<script lang="ts">
  import {
    connected,
    web3,
    selectedAccount,
    chainId,
    chainData,
    defaultEvmStores,
  } from "svelte-web3";
  import { onMount } from "svelte";

  onMount(() => {
    defaultEvmStores.setProvider();
  });
</script>

<main>
  <h1>New web3js 4.x.x seems problematic..</h1>
  <p>Check console</p>
</main>

<style>
</style>

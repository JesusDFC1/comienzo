<script>
  import Paises from "./lib/paises.svelte";
  const lista = ["colombia", "venezuela", "ecuador", "peru", "brasil", "argentina", "bolivia","chile","paraguay","uruguay","surinam", "ganauy", "trinidad y tobago" ];
</script>

<div class="main">
  {#each lista as pais}
  <div>
    <Paises pais={pais} />
  </div>
    
  {:else}
    <p>No existen elementos</p>
  {/each}
</div>

<svelte:head>
  <title>PAÍSES DE SUDAMÉRICA</title>
</svelte:head>

<style>
  .main {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-gap: 10px;
    grid-auto-rows: minmax(100px, auto);
  }
</style>

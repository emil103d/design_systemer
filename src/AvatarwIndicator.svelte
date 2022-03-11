<script>
  import Badge from "./Badge.svelte";
  import Button from "./Button.svelte";
  export let type;
  export let name;
  export let mode;
  export let image = true;
</script>

<div class="container {type}">
  <div class:indicator={mode === "indicator"} />
  <div />
  {#if image === true}
    <img src="sko.png" alt="" />
  {:else}
    <p>{name}</p>
  {/if}
</div>

<style>
  p {
    color: white;
  }

  img {
    height: 100%;
    width: 100%;
    border-radius: 100%;
  }

  .container {
    width: 8rem;
    height: 8rem;
    border-radius: 8rem;
    background: var(--default-color);
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 2rem;
    position: relative;
  }

  .indicator {
    width: 15%;
    height: 15%;
    border-radius: 100%;
    background: var(--accent-color);
    position: absolute;
    right: 8%;
    top: 0%;
    border: solid 2px white;
  }

  .large {
    width: 8rem;
    height: 8rem;
    border-radius: 100%;
    font-size: 2rem;
  }

  .medium {
    width: 6rem;
    height: 6rem;
    border-radius: 100%;
    font-size: 1.5rem;
  }

  .small {
    width: 4rem;
    height: 4rem;
    border-radius: 100%;
    font-size: 1rem;
  }

  .x-small {
    width: 2rem;
    height: 2rem;
    border-radius: 100%;
    font-size: 0.5rem;
  }
</style>

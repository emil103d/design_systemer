<script>
  export let type = "default";
</script>

<div class={type}><slot /></div>

<style>
  div {
    /* all: unset; */
    color: var(--primary-font-color);
    background: var(--default-color);
    padding: 0.5rem;
    border-radius: 15px;
    transition: all 0.2s;
    cursor: pointer;
    font-size: 0.7rem;
    font-weight: 600;
    display: inline-block;
  }

  div:hover {
    filter: brightness(1.5);
  }

  .primary {
    background-color: var(--primary-color);
  }

  /* .primary.inversed {
    color: var(--ghost-color);
    background: var(--primary-font-color);
  } */

  .secondary {
    background-color: var(--secondary-color);
  }

  .ghost {
    color: var(--ghost-color);
    background: var(--primary-font-color);
  }

  /* .secondary.inversed {
    color: var(--link-color);
    background: var(--primary-font-color);
  } */

  .accent {
    background-color: var(--accent-color);
  }

  .categori {
    color: var(--ghost-color);
    background-color: white;
    border: solid 1px var(--ghost-color);
  }
</style>

<script>
  export let type = "default";
  export let mode;
</script>

<button class:inversed={mode === "inversed"} class={type}><slot /></button>

<style>
  button {
    /* all: unset; */
    border: none;
    color: var(--primary-font-color);
    background: var(--default-color);
    padding: 1rem;
    border-radius: 10px;
    transition: all 0.2s;
    cursor: pointer;
    text-transform: uppercase;
    font-size: 0.7rem;
    font-weight: 600;
  }

  button:hover {
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

  .link {
    color: var(--link-color);
    background: var(--primary-font-color);
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
</style>

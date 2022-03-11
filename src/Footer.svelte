<script>
  export let links1;
  export let links2;
  export let links3;
</script>

<footer>
  <div>
    <h4>Serivce</h4>
    {#each links1 as link}
      <a href="#0">{link}</a>
    {/each}
  </div>
  <div>
    <h4>Comapny</h4>
    {#each links2 as link}
      <a href="#0">{link}</a>
    {/each}
  </div>
  <div>
    <h4>Legal</h4>
    {#each links3 as link}
      <a href="#0">{link}</a>
    {/each}
  </div>
</footer>

<style>
  footer {
    display: grid;
    background: #3f444f;
    color: white;
    font-weight: 400;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    padding: 2rem;
    margin: 0;
    font-size: 0.8rem;
  }

  a {
    all: unset;
    display: block;
    padding: 0.3rem;
  }

  h4 {
    color: grey;
    font-weight: 600;
    text-transform: uppercase;
  }
</style>

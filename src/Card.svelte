<script>
  export let title;
  import Badge from "./Badge.svelte";
  import Button from "./Button.svelte";
</script>

<article>
  <img src="sko.png" alt="" />
  <div class="container">
    <h3>{title} <Badge type="secondary">NEW</Badge></h3>
    <p>If a dog chews whose shoes does he choose?</p>
    <div>
      <Badge type="categori">Fashion</Badge>
      <Badge type="categori">Products</Badge>
    </div>
    <div class="button">
      <Button type="primary">Buy now</Button>
    </div>
  </div>
</article>

<style>
  article {
    width: 20rem;
    box-shadow: rgba(0, 0, 0, 0.2) 0px 18px 50px -10px;
    border-radius: 10px;
    flex-direction: column;
  }

  .container {
    padding: 1rem;
  }

  img {
    border-radius: 12px 12px 0px 0px;
    width: 100%;
    margin: 0;
  }

  .button {
    text-align: right;
    padding-top: 0.5rem;
  }
</style>

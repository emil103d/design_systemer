<script>
  import Button from "./Button.svelte";
  export let title;
</script>

<div class="container">
  <Button type="default"
    >{title}
    <div class="badge"><slot /></div></Button
  >
</div>

<style>
  .container {
    position: relative;
    display: inline-block;
  }

  .badge {
    position: absolute;
    top: -13px;
    right: -16px;
  }
</style>

<script>
  export let step
  export let index
</script>

<input type="text" value={step.text}/><img src="/images/add.png" alt="Add" width="24" height="24" />
{#if (step.image != '')}
  <img class="screenshot" src={step.image} width="500" alt="ui display"/>
{/if}

<style>

  img {
    left: 534px;
  }

  img.screenshot {
    display: block;
    top: 4px;
    left: 0;
    border-radius: 4px;
    box-shadow: 3px 3px 2px gray;
    margin-top: 10px;
    margin-bottom: 10px;
  }
</style>
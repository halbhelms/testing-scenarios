<script>
  export let step
  export let index
</script>

<input type="text" value={step.text}/><img src="src/lib/images/add.png" alt="Add" width="24" height="24" />
{#if (step.image != '')}
  <img class="screenshot" src={step.image} width="500" alt="ui display"/>
{/if}

<style>
  p {
    width: 500px;
    padding: 4px;
    background-color: white;
    font-family: 'Shadows Into Light Two', sans-serif;
    margin-bottom: -30px;
    border-radius: 4px;
  }

  img {
    position: relative;
    top: 4px;
    left: 504px;
  }

  img.screenshot {
    display: block;
    top: 4px;
    left: 0;
    border-radius: 4px;
    box-shadow: 3px 3px 2px gray;
  }
</style>
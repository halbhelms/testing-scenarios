<script>
  export let scenario
  import Step from '$lib/components/Step.svelte'
  let sortedSteps = scenario.steps
</script>

<main>
<label for="steps">Steps</label>
<div id="steps" name="steps">
  {#each sortedSteps as step, index}
    <Step {step} {index}/>
  {/each}
</div>
</main>
<style>
div {
  display: inline-block
}

main {
  background-color: #D2D0C3;
  position: relative;
  margin: 0 auto;
  padding: 10px;
}

label {
  display: inline-block;
  width: 200px;
  text-align: right;
  margin-left: 20px;
  margin-right: 6px;
  vertical-align: top;
}
</style>
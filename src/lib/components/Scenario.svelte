<script>
  export let scenario
</script>

<main>
  <label for="name">Scenario Name</label>
  <input type="text" id="name" name="name" bind:value={scenario.name} />
</main>

<style>
  main {
  background-color: #D2D0C3;
  /* color: #fff; */
  position: relative;
  margin: 0 auto;
  padding: 10px;
}
</style>
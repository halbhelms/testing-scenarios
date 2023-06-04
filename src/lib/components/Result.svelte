<script>
  export let scenario
</script>

<main>
  <label for="result">Scenario Result</label>
  <select name="result" id="result" value="{scenario.result}">
    <option value="none">The test...</option>
    <option value="pass">passed</option>
    <option value="fail">failed</option>
    <option value="blocked">passed w/problems</option>
  </main>

<style>
  main {
    background-color: #D2D0C3;
    position: relative;
    margin: 0 auto;
    padding: 10px;
  }

</style>

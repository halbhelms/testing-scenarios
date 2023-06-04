<script>
  export let scenario
</script>

<main>
  <label for="brief">Scenario Brief</label>
  <textarea id="brief" name="brief" value="{scenario.brief}" />
</main>

<style>
  main {
    background-color: #C3C6D2;
    position: relative;
    margin: 0 auto;
    padding: 10px;
  }
  textarea {
    width: 500px;
    height: 75px;
    border-radius: 4px;
    border: 1px solid lightgray;
    padding: 4px;
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
<script>
  let scenario = {
    name: 'Sample Scenario',
    brief: '',
    steps: [
      {id: 1, text: '', image: 'step1.png'},
      {id: 2, text: '', image: ''},
    ] ,
    expectation: '',
    result: 'none',
    image: '', 
    notes: ''
  }
  import { enhance } from '$app/forms'

  import Scenario from '$lib/components/Scenario.svelte'
  import Brief from '$lib/components/Brief.svelte'
  import Steps from '$lib/components/Steps.svelte'
  import Expectation from '$lib/components/Expectation.svelte'
  import Result from '$lib/components/Result.svelte'
  import Image from '$lib/components/Image.svelte'
  import Notes from '$lib/components/Notes.svelte'

  export let form
</script>

<main>
  <h1>New Scenario</h1>
  <form method="post" use:enhance|preventDefault enctype="multipart/form-data">
    <input type="file" name="file" />
  <Scenario {scenario} />
  <Brief {scenario} />
  <Steps {scenario} />
  <Expectation {scenario} />
  <Result {scenario} />
  <Image {scenario} />
  <Notes {scenario} />
  <button>Save Scenario</button>
  </form>
</main>

<style>
  button {
    display: block;
    margin: 10px auto;
  }
</style>
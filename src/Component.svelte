<script>
  export let name;
  export let buttonText = "Button";

  function handleClick() {
    buttonText += " Clicked";
  }
</script>

<svelte:options tag="my-counter" />

<!-- your code here -->
<h1>Hello {name}!</h1>

<button on:click={handleClick}>{buttonText}</button>

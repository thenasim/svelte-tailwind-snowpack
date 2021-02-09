<script>
  import "./tailwind.svelte";
  let count = 0;

  function handleClick() {
    count += 1;
  }
</script>

<div class="flex justify-center items-center w-full h-screen">
  <div>
    <button class="primary" type="button" on:click={handleClick}>
      Clicked {count}
      {count === 1 ? "time" : "times"}
    </button>
  </div>
</div>

<style>
  .primary {
    @apply p-3 bg-gray-100 rounded-md focus:outline-none focus:ring focus:ring-gray-200;
  }
</style>

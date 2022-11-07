

<!-- Javascript -->

<script>
  
  // Declare a new variable
  let counter = 0;

  // Create a new function
  function incrementCounter() {
    counter++;
  }

  // Create a new list
  let myList = [1, 2, 3, 4, 5];

</script>


<!-- HTML -->
<main>

  <!-- Using Headers -->
  <h1 class="my_header">Header1 Title</h1>
  <h2>Header2 Title #1</h2>
  <h2>Header2 Title #2</h2>

  <!-- Using Buttons -->
  <button on:click={() => {
    
    // Call the incrementCounter() function
    incrementCounter();
    // or just do
    counter++;
  
  }}>
  
  Click to Increment Counter

  </button>


  <h3>Counter: {counter}</h3>


  <!-- Using Paragraphs-->
  <p>This is a paragraph</p>


  <!-- Using Divs -->
  <div id="my_div">
      <p>This is a paragraph wrapped in a div</p>
  </div>



  <!-- Loop over that items in the myList variable-->
  {#each myList as value}

  
    <!-- If statements-->
    {#if value == 1}
      <h2>Value is equal to one</h2>

    {:else if value == 2}
      <h2>Value is equal to two</h2>
    
    {:else}
      <h2>Value is {value}</h2>


    <!-- End of the if statement -->
    {/if}


  <!-- End of the loop -->
  {/each}


</main>


<!-- CSS -->
<style>

  /* Using Styling IDS */
  #my_div {
    background-color: blue;
  }

  /* Using Styling Classes */
  .my_header {
    color: green;
  }

  /* Styling Every 'h2' Elements */
  h2 {
    /* Use RGB */
    color: rgb(255, 0, 0);
  }
  
</style>

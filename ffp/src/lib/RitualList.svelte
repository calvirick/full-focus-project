<script>
  let listItems = [
    "MORNING RITUAL",
    "WORKDAY STARTUP RITUAL",
    "WORKDAY SHUTDOWN RITUAL",
    "EVENING RITUAL",
  ];
</script>

{#each listItems as listItem}
  <ul><li>{listItem}</li></ul>
{/each}

<style>
  ul {
    list-style-type: none;
    display: flex;
  }
  /* Circles */
  li:before {
    content: "◯";
    margin-right: 20px;
    font-weight: bold;
  }
</style>

<script>
  let quarters = [13, 12, 11, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0];
</script>

<div id="top" class="container">
  <p>Weeks Remaining in Quarter</p>
  <ol>
    {#each quarters as quarter}
      <span><strong>{quarter}</strong></span>
    {/each}
  </ol>
</div>

<style>
  @media (min-width: 739px) {
    .container {
      display: flex;
      justify-content: center;
      align-items: center;
    }
  }

  ol {
    list-style-type: none;
    display: flex;
    justify-content: center;
    padding-right: 40px;
    margin: 0 5px;
    max-width: 500px;
    /* border: solid green 1px; */
  }

  span {
    margin: 0 auto;
    /* border: solid red 1px; */
    width: 1.6rem;
    height: 1.6rem;
    border-radius: 100%;
    align-items: center;
    line-height: 1.8rem;
  }

  span:hover {
    color: white;
    cursor: pointer;
    background-color: #8c8c8c;
  }
</style>

<script>
  export let images;
</script>

<div class="layout">
  {#each images as image}
  <div class="layout__item">
    <img src="{image.src}" alt=""/>
  </div>
  {/each}
</div>

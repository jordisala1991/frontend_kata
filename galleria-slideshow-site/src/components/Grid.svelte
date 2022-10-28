<script>
  export let images;

  const columnSize = Math.ceil(images.length / 4);
  const lastColumnSize = Math.floor(images.length % 4);
  const totalColumns = 4;
</script>

<div class="layout">
  {#each Array(totalColumns) as _, i}
    <div class="layout__column">
      {#each Array(columnSize) as _, j}
        <div class="layout__item">
          <img src="{images[i + j].src}" alt=""/>
        </div>
      {/each}
    </div>
  {/each}
</div>

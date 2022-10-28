<script>
  import Header from './components/Header.svelte'
  import Grid from './components/Grid.svelte';
  import data from './data.json';

  const images = data.map(block => ({
    src: block.images.thumbnail
  }));
</script>

<main>
    <Header />
  <Grid images={images}/>
</main>

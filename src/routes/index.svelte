<script>
  import successkid from "images/successkid.jpg";
  import Carousel from "@beyonk/svelte-carousel";
</script>

<svelte:head>
  <title>Sapper project template</title>
</svelte:head>

<h1>Great success!</h1>

<figure>
  <img alt="Success Kid" src={successkid} />
  <figcaption>Have fun with Sapper!</figcaption>
</figure>
<Carousel perPage={{ 800: 2, 500: 2 }}>
  <div class="slide-content">
    <img src="//placekitten.com/401" alt="Kitten 1" />
  </div>
  <div class="slide-content">
    <img src="//placekitten.com/401" alt="Kitten 1" />
  </div>
  <div class="slide-content">
    <img src="//placekitten.com/402" alt="Kitten 1" />
  </div>
  <div class="slide-content">
    <img src="//placekitten.com/403" alt="Kitten 1" />
  </div>
</Carousel>
<p>
  <strong
    >Try editing this file (src/routes/index.svelte) to test live reloading.</strong
  >
</p>

<style>
  :global(img) {
    opacity: 0.9;
    transition: all 0.2s;
  }
  :global(img):hover {
    opacity: 1;
    transform: scale(1.04);
  }
  h1,
  figure,
  p {
    text-align: center;
    margin: 0 auto;
  }

  h1 {
    font-size: 2.8em;
    text-transform: uppercase;
    font-weight: 700;
    margin: 0 0 0.5em 0;
  }

  figure {
    margin: 0 0 1em 0;
  }

  img {
    width: 100%;
    max-width: 400px;
    margin: 0 0 1em 0;
  }

  p {
    margin: 1em auto;
  }

  .slide-content {
    width: 100%;
    height: 100%;
  }

  iframe {
  }

  @media (min-width: 480px) {
    h1 {
      font-size: 4em;
    }
  }
</style>

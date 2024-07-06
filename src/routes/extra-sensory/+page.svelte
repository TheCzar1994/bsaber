<script>
  import MetaHead from '$lib/MetaHead.svelte'
  import MapCards from '$lib/MapCards.svelte'
</script>

<MetaHead
  title="Extra Sensory I"
  description="EXTRA SENSORY I - The original Extra Sensory event pack release which debuted in 2020"
  imageUrl="/totalbslogo1.png"
/>

<section class="hero">
  <div class="content">
    <p>
      <img src="/totalbslogo1.png" alt="TotalBS Logo" width="100" height="100" />
    </p>
    <p>TOTAL BS PRESENTS</p>
    <h1>EXTRA SENSORY I</h1>
    <p>
      Time for something you've never seen before!
      <br />
      <br />
      The Extra Sensory event saw the release of five new maps that use the game in new, creative ways
      that will flip how you play on its head. This song pack contains all of them in one place for you!
      From hell to cities, hitting bombs and notes that can't sit still, you're sure to find a new unexpected
      experience here.
    </p>
    <div class="buttons">
      <a class="btn" href="https://api.beatsaver.com/playlists/id/50/download" target="_blank"
        >DOWNLOAD</a
      >
      <a
        class="btn2"
        href="https://beatmods.com/uploads/6600b82cdfb5962c5bb29d42/universal/NoodleExtensions-1.6.1.zip"
        target="_blank">NOODLE EXTENSIONS</a
      >
      <a
        class="btn3"
        href="https://beatmods.com/uploads/6600b865dfb5962c5bb29d45/universal/Chroma-2.8.1.zip"
        target="_blank">CHROMA</a
      >
    </div>
  </div>
</section>
<br />
<h2>Download the maps below!</h2>
<hr class="fade" />
<MapCards playlistId="50" />

<style lang="scss">
  @import 'src/scss/variables';
  .hero {
    position: relative;
    min-height: 55rem;
    height: 70vh;
    background-size: cover;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    margin-top: -28px;
    overflow: hidden;
  }

  .hero::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: url('/totalbsbackground.png') no-repeat center center;
    background-size: cover;
    filter: brightness(30%) blur(5px);
    z-index: -1;
  }

  .content {
    position: relative;
    z-index: 1;
    bottom: 10rem;
  }

  h1 {
    font-size: 3.5rem;
    width: 100%;
    justify-content: center;
    text-align: center;
    margin-top: 2rem;
  }
  @media (max-width: 678px) {
    h1 {
      font-size: 2.5rem;
    }
  }
  @media (max-width: 400px) {
    h1 {
      font-size: 1.5rem;
    }
  }

  p {
    margin: 0.5rem 1rem 0;
    font-weight: 600;
    font-size: large;
  }
  .btn,
  .btn2,
  .btn3 {
    border: none;
    padding: 12px 30px;
    cursor: pointer;
    font-size: 15px;
    position: absolute;
    text-align: center;
    width: 165px;
    justify-content: center;
    transition: background-color 0.5s ease;
    border-radius: 5px;
    font-weight: bolder;
  }

  .btn:hover,
  .btn2:hover,
  .btn3:hover {
    background-color: #5d5d8b;
    text-decoration: none;
    color: white;
  }

  .btn {
    background-color: #0cc0c9;
    color: white;
    top: 125%;
    left: 50%;
    transform: translate(-50%, -50%);
  }

  .btn2 {
    background-color: #0cc0c9;
    color: white;
    top: 140%;
    left: 50%;
    transform: translate(-50%, -50%);
  }

  .btn3 {
    background-color: #0cc0c9;
    color: white;
    top: 155%;
    left: 50%;
    transform: translate(-50%, -50%);
  }

  hr.fade {
    border: none;
    height: 2px;
    margin-block: 0.75rem 1.5rem;
    background: linear-gradient(90deg, #999999 0%, rgba(153, 153, 153, 0) 100%);
  }
</style>

<script>
  import MetaHead from '$lib/MetaHead.svelte'
  import MapCards from '$lib/MapCards.svelte'
</script>

<MetaHead
  title="Fox Stevenson Pack"
  description="Alphabeat presents their newest pack, featuring songs by Fox Stevenson (formerly Stan SB / Stan SSB)!"
  imageUrl="/uploads/playlists/fox-red.png"
/>

<section class="hero">
  <div class="content">
    <div class="card-container">
      <div class="card">
        <a href="https://beatsaver.com/profile/5122" target="_blank"
          ><img src="/uploads/playlists/alphabeat1.jpg" alt="Alphabeat" />
        </a>
      </div>
    </div>
    <div class="uploader-container">
      <a class="uploader" href="https://beatsaver.com/profile/5122" target="_blank">Alphabeat</a>
      Presents
    </div>
    <div class="body">
      <h1>Fox Stevenson Pack</h1>
      <p>
        Alphabeat presents their newest pack, featuring songs by Fox Stevenson (formerly Stan SB /
        Stan SSB)!
        <br />
        He is an English singer-songwriter, DJ and producer of bass music, mostly drum and bass and glitch
        hop.
        <br />
        We hope you enjoy!
      </p>
    </div>
    <div class="buttons">
      <a class="btn" href="https://api.beatsaver.com/playlists/id/581099/download" target="_blank"
        >ZIP DOWNLOAD</a
      >
      <a class="btn2" href="https://beatsaver.com/playlists/581099" target="_blank">BEATSAVER</a>
    </div>
  </div>
</section>
<br />
<h2>Download the maps below!</h2>
<hr class="fade" />
<MapCards playlistId="581099" />

<style>
  .hero {
    position: relative;
    min-height: 45rem;
    height: 70vh;
    background-size: cover;
    margin-top: -20px;
    overflow: hidden;
  }
  .hero::before {
    content: '';
    position: absolute;
    width: 100%;
    height: 100%;
    background: url('/uploads/playlists/fox-red.png') no-repeat center center;
    background-size: cover;
    filter: brightness(30%) blur(5px);
    z-index: -1;
  }

  .content {
    display: flex;
    flex-direction: column;
    position: absolute;
    justify-content: center;
    text-align: center;
    align-items: center;
    z-index: 1;
    width: 100%;
    height: 100%;
  }

  .card-container {
    display: flex;
    gap: 2.5rem;
    height: 200px;
    transform: scale(15%);
    margin-top: -5rem;
  }
  .card {
    height: 700px;
    background: rgba(0, 0, 0, 0);
    flex: 1;
    width: 45rem;
  }
  .card img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-radius: 25px;
  }

  .uploader {
    color: white;
    font-weight: 1000;
  }

  .body {
    padding-bottom: 2.5rem;
  }

  h1 {
    font-size: 3.5rem;
    width: 100%;
    justify-content: center;
    text-align: center;
    margin-top: 1rem;
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
    margin: 0.5rem 0.5rem 0;
  }

  .buttons {
    display: grid;
    gap: 0.5rem;
    justify-content: center;
    width: 100%;
  }
  .btn,
  .btn2 {
    padding: 12px 30px;
    cursor: pointer;
    font-size: 15px;
    text-align: center;
    transition: background-color 0.5s ease;
    border-radius: 5px;
    font-weight: bolder;
    width: 165px;
  }

  .btn:hover {
    background-color: #4c0000;
    text-decoration: none;
    color: white;
  }
  .btn2:hover {
    background-color: #4c0000;
    text-decoration: none;
    color: white;
  }

  .btn {
    background-color: #fffdfd;
    color: black;
  }

  .btn2 {
    background-color: #fffdfd;
    color: black;
  }

  hr.fade {
    border: none;
    height: 2px;
    margin-block: 0.75rem 1.5rem;
    background: linear-gradient(90deg, #999999 0%, rgba(153, 153, 153, 0) 100%);
  }
</style>

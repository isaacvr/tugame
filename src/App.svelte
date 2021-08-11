<script type="ts">
  import banner from './assets/banner.png';
  import Search from './Search.svelte';

  let cards = [
    { name: "Assassin Creed", img: "src/assets/ac.webp", },
    { name: "Mortal Kombat",  img: "src/assets/mc.jpeg", },
    { name: "Forged Fantasy", img: "src/assets/ff.jpg", },
    { name: "Sniper Elite 4", img: "src/assets/se4.webp", },
  ];
</script>

<div class="banner">
  <img class="banner-img" src={banner} alt="Fornite">

  <div class="cell">
    <span class="title">Tugame</span>
    <Search></Search>
  </div>
  <div class="cell">
    <h1>Get your phone ready for the battle, it's starting now</h1>
  </div>
  <div class="cell">
    <button>
      <svg aria-label="Google Play" id="Layer_1" style="enable-background:new 0 0 24 24;" version="1.1" viewBox="0 0 24 24" xml:space="preserve" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"><g><g><path d="M3.713,23.015c-0.34,0-0.679-0.091-0.986-0.273c-0.594-0.352-0.949-0.975-0.949-1.666V2.924    c0-0.691,0.355-1.314,0.949-1.666c0.595-0.352,1.312-0.364,1.917-0.032l16.573,9.076c0.63,0.345,1.006,0.98,1.006,1.698    s-0.376,1.354-1.006,1.698L4.644,22.774C4.35,22.934,4.031,23.015,3.713,23.015z M3.713,1.987c-0.165,0-0.329,0.044-0.477,0.132    C2.948,2.289,2.777,2.59,2.777,2.924v18.151c0,0.334,0.171,0.635,0.459,0.806c0.288,0.169,0.634,0.175,0.927,0.016l16.573-9.076    c0.305-0.167,0.487-0.474,0.487-0.821s-0.182-0.654-0.487-0.821L4.163,2.103C4.022,2.025,3.867,1.987,3.713,1.987z"/></g><g><path d="M16.777,15.5c-0.125,0-0.25-0.046-0.347-0.14l-13.5-13C2.731,2.168,2.725,1.852,2.917,1.653    c0.192-0.199,0.51-0.204,0.707-0.014l13.5,13c0.199,0.192,0.205,0.508,0.014,0.707C17.039,15.449,16.908,15.5,16.777,15.5z"/></g><g><path d="M3.277,22.5c-0.131,0-0.262-0.051-0.36-0.153c-0.191-0.199-0.186-0.515,0.014-0.707l13.5-13    c0.198-0.19,0.516-0.186,0.707,0.014c0.191,0.199,0.186,0.515-0.014,0.707l-13.5,13C3.527,22.454,3.402,22.5,3.277,22.5z"/></g></g><g/><g/><g/><g/><g/><g/><g/><g/><g/><g/><g/><g/><g/><g/><g/></svg>
      Play Store
    </button>
    <button>
      <svg aria-label="App Store" enable-background="new 0 0 24 24" height="24px" id="Layer_1" version="1.1" viewBox="0 0 24 24" width="24px" xml:space="preserve" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"><g><polygon points="2.7,22.8 4.2,21.8 2.9,21  "/><path d="M12.5,7.8l-1.6-0.9c0,0,0,0-0.1,0c0,0-0.1,0-0.1,0l-7.4,13l0,0.2L5,21C5,21,5,21,5.1,21l7.4-13C12.5,7.9,12.5,7.9,12.5,7.8   z"/><path d="M6.9,11.5H1.6l-0.1,2.9c0,0.1,0.1,0.3,0.1,0.4H5L6.9,11.5z"/><path d="M20.7,20.2l-0.4,0.3c0,0,0,0,0,0c-0.2,0.2-0.2,0.4,0.1,0.9c0.3,0.4,0.8,0.6,1.3,0.8c0.1,0,0.2,0.1,0.3,0.1   c0-0.8-0.2-1.6-0.5-2C21.3,20.2,21,20.1,20.7,20.2z"/><path d="M11.7,11.5l-1.9,3.3h5.6c-0.4-0.8-0.9-1.9-1.5-3.3H11.7z"/><path d="M17.8,11.5c0.1,0.3,0.3,0.5,0.4,0.8l0.5,1l0.1,0.1l0.7,1.2c0,0.1,0.1,0.1,0.1,0.2h2.7c0.1-0.1,0.1-0.3,0.1-0.4v-2.9   L17.8,11.5z"/><path d="M20.4,19.3c0.1-0.1,0.1-0.2,0.1-0.3l-0.8-1.5c0-0.1-0.1-0.1-0.2-0.1l-0.3,0.2c-0.1,0.1-0.2,0.1-0.4,0.2l-0.1,0.1   c0,0,0,0-0.1,0l-0.1,0.1c-0.1,0.1-0.1,0.1,0,0.2l1,1.5c0,0.1,0.1,0.1,0.2,0.1c0,0,0,0,0,0c0,0,0,0,0,0c0,0,0.1-0.1,0.1-0.1   c0.1-0.1,0.2-0.1,0.3-0.1L20.4,19.3z"/><path d="M19.1,16.3c0-0.1,0-0.1,0-0.3c0,0,0-0.1,0-0.1c-0.1-0.1-0.2-0.4-0.4-0.8l-0.6-1.2c0,0,0-0.1,0-0.1l-0.1-0.1   c0-0.1-0.1-0.1-0.1-0.2l-0.3-0.6c0,0,0-0.1-0.1-0.1c-1.6-3-2.7-5-3.4-6.1c-0.5-0.7-0.9-1.6-1.4-2.4c-0.6-1-1.3-2.3-1.9-3.1   c0.3,1.3,1.5,3.9,2,5.1l0.2,0.5c0,0.1,0,0.1,0,0.2L13,7c0.4,0.3,0.6,0.8,0.5,1.2c0,0,0,0,0,0c2,4.7,3.8,8.3,4.2,8.7   c0.3,0.1,0.4,0.1,0.6,0l0.6-0.3C18.9,16.5,19.1,16.4,19.1,16.3z"/></g></svg>
      App Store
    </button>
  </div>
  <div class="auth">
    <button>sign in</button>
    <button>sign up</button>
  </div>
</div>

<ul class="card-list">
  {#each cards as card}
    <li class="card">
      <div class="img-container">
        <img src={card.img} alt={card.name}>
      </div>
      <div class="info">
        <span class="name">{card.name}</span>
        <div class="stars">
          <div class="star"></div>
          <div class="star"></div>
          <div class="star"></div>
          <div class="star"></div>
          <div class="star"></div>
        </div>
      </div>
    </li>
  {/each}
</ul>


<style>
  .banner {
    background: linear-gradient(to right, #3c0163, #a659e0);
    margin: 2rem 3rem;
    border-radius: 3rem;
    padding: 2rem 4rem;
    position: relative;
    z-index: 1;
    color: #fcd6ff;
    display: grid;
    height: 38rem;
    box-shadow: 0px 16px 3rem #7008b7c2;
  }

  .banner .banner-img {
    position: absolute;
    z-index: -1;
    right: 7%;
    display: flex;
    margin-block: auto;
    top: 0;
    bottom: 0;
    mix-blend-mode: hard-light;
    height: 90%;
  }

  .banner .title {
    font-size: 1.8rem;
    margin-top: 1.8rem;
  }

  .banner .cell button {
    border: none;
    padding: 1.43rem 1rem;
    color: white;
    font-size: 1.3rem;
    border-radius: 1rem;
    margin-right: 1rem;
    top: 2rem;
    position: relative;
    cursor: pointer;
    transform-style: preserve-3d;
    transition: all 300ms;
    display: inline-flex;
    align-items: center;
    width: 13rem;
    justify-content: space-around;
  }

  .banner .cell button:hover {
    box-shadow: 0px 9px 18px rgba(0, 0, 0, 0.4);
    transform: translateY(-9px) rotate(4deg);
  }

  .banner .cell button:nth-child(1) {
    background: linear-gradient(to right, #64268b, #6c2f97);
  }

  .banner .cell button:nth-child(2) {
    background: linear-gradient(to right, #70329d, #7a3aa8);
  }

  .banner .cell button svg {
    width: 3rem;
    height: 3rem;
    fill: currentColor;
  }

  .banner .cell:nth-of-type(1) {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
  }

  .banner h1 {
    max-width: 24ch;
    font-size: 3.1rem;
    text-transform: capitalize;
    line-height: 5.6rem;
    font-weight: 900;
    text-shadow: 0px 0px 10px rgba(0, 0, 0, .3);
  }

  .banner .auth {
    position: absolute;
    right: 0;
    transform: rotate(-90deg);
    display: flex;
    align-items: center;
    top: 0;
    bottom: 0;
    height: 0;
    margin: auto;
  }

  .banner .auth button {
    color: #edb0fe;
    background-color: transparent;
    border: none;
    margin-right: 1rem;
    margin-bottom: -5rem;
    font-size: 1.4rem;
    font-weight: bold;
    cursor: pointer;
    transition: all 300ms;
  }

  .banner .auth button:hover {
    color: #f8b8b8;
  }

  .card-list {
    list-style: none;
    margin: 2rem 3rem;
    padding: 0;
    width: calc(100% - 6rem);
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-gap: 3rem;
    margin-top: 4rem;
  }

  .card-list .card {
    border-radius: .7rem;
    background-color: #e8e8e8;
  }

  .card-list .card .img-container {
    position: relative;
    width: calc(100% - 2rem);
    height: 0;
    padding-top: calc(100% - 2rem);
    display: flex;
    margin: 0 auto;
    margin-bottom: 2rem;
    margin-top: 1rem;
    overflow: hidden;
    cursor: pointer;
  }

  .card-list .card .img-container:hover img {
    transform: scale(1.2) rotate(3deg);
  }

  .card-list .card img {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: center;
    border-radius: .7rem;
    transition: all 700ms;
  }

  .card-list .card .info {
    display: grid;
    grid-template-columns: 1fr 1fr;
    padding: 0 1rem;
  } 

  .card-list .card .info .name {
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
    margin-bottom: 1rem;
  }

  .card-list .card .info .stars{
    display: flex;
    margin-left: auto;
  }

  .card-list .card .info .stars .star{
    width: 1.3rem;
    height: 1.3rem;
    clip-path: polygon(50% 0%, 61% 35%, 98% 35%, 68% 57%, 79% 91%, 50% 70%, 21% 91%, 32% 57%, 2% 35%, 39% 35%);
    background-color: #cabd00;
    cursor: pointer;
  }
</style>
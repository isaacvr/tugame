<script>
  import search from './assets/Search.svg';
</script>

<div class="search-container">
  <img src={search} alt="">
  <input type="search" placeholder="Search..." aria-label="Search">
</div>

<style>
  .search-container {
    background-color: #955dc0;
    color: lightgray;
    height: 4.5rem;
    border-radius: 1rem;
    position: relative;
    transition: all 300ms;
  }

  .search-container:focus-within {
    background-color: #4f0f81;
    color: #d9d9d9;
    outline: 1px solid #ffffff5c;
  }

  .search-container img {
    position: absolute;
    top: 0;
    bottom: 0;
    display: flex;
    margin-block: auto;
    margin-left: 2rem;
    transform: scaleX(-1);
    filter: invert(.8);
    width: 2rem;
    height: 2rem;
  }

  .search-container input {
    position: relative;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: transparent;
    border: none;
    outline: none;
    color: currentColor;
    font-size: 1.5rem;
    padding-left: 5rem;
  }

  .search-container input:focus {
    color: currentColor;
  }
</style>
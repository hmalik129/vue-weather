<template>
<div class="app">
  <main>
    <div class="search-box">
      <input type="text" class="search-bar" placeholder="Search..."/>
    </div>
    <div class="weather-wrap">
      <div class="location-box">
        <div class="location">Niagara Falls, Canada</div>
        <div class="date">Friday, May 5, 2020</div>
      </div>

      <div class="weather-box">
        <div class="temp">9°</div>
        <div class="weather">Rain</div>
      </div>
    </div>
  </main>
</div>
</template>

<script>

export default {
  name: 'App',
  data () {
    return {
      api_key: '4be35d29534395fbf9da77cc42e02afe'
    }
  }

}
</script>

<style>

*{      
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'montserrat', sans-serif;
}

#app {
  background-image: url('./assets/cold-bg.jpg');
  background-size: cover;
  background-position: bottom;
  transition: 0.4s;
}

main {
  min-height: 100vh;
  padding: 30px;

  background-image: linear-gradient(to bottom, rgba(0,0,0,0.15), rgba(0,0,0,0.65));
}

.search-box {
  width: 100%;
  margin-bottom: 30px;
}

.search-box .search-bar {
  display: block;
  width: 100%;
  padding: 15px;

  color: #dd0808;   /* Font Color */
  font-size: 20px;

  appearance: none;   
  border: none;
  outline: none;
  background: none;

  box-shadow: 0px, 0px 8px, rgba(0, 0, 0, 0.25);
  background-color: rgba(255, 255, 255, 0.5);
  border-radius: 16px 0px 16px 0px;
  transition: 0.4s;
}

.search-box .search-bar:focus {
  box-shadow: 0px 0px 16px rgba(0, 0, 0, 0.25);
  background-color: rgba(255, 255, 255, 0.75);
  border-radius: 0px 16px 0px 16px;
}

</style>

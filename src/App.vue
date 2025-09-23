<script setup>
import FilterControls from './components/FilterControls.vue'
import Navbar from './components/Navbar.vue'
import PlayerBar from './components/PlayerBar.vue'
import Playlist from './components/Playlist.vue'
import Track from './components/Track.vue'
</script>

<template>
  <div class="wrapper">
    <div class="container">
      <main class="main">
        <Navbar />
        <div class="main__centerblock centerblock">
          <div class="centerblock__search search">
            <svg class="search__svg">
              <use xlink:href="/img/icon/sprite.svg#icon-search"></use>
            </svg>
            <input class="search__text" type="search" placeholder="Поиск" name="search" />
          </div>
          <FilterControls />
          <Playlist />
        </div>
        <Track />
      </main>
      <PlayerBar />
      <footer class="footer"></footer>
    </div>
  </div>
</template>

<style scoped></style>
